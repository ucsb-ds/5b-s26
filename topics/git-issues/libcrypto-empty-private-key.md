---
title: "Load key error in libcrypto"
permalink: "/git-issues/libcrypto-empty-private-key"
layout: default
parent: Git Issues
grand_parent: Topics
nav_order: 4
---

# Load key error in libcrypto

## If your screen looks like this

```text
jovyan@jupyter-rachitgupta:~$ git clone git@github.com:ucsb-cs5b-s26/lab01-rachit182.git
Cloning into 'lab01-rachit182'...
Load key "/home/jovyan/.ssh/id_ed25519": error in libcrypto
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
```

## What this usually means

Your SSH private key file exists, but it is empty or corrupted.

For example, you may see something like this:

```text
jovyan@jupyter-rachitgupta:~$ ls -l ~/.ssh
total 8
-rwx------. 1 jovyan users   0 Apr  1 19:38 id_ed25519
-rwx------. 1 jovyan users 108 Apr  1 18:22 id_ed25519.pub
-rwx------. 1 jovyan users 142 Apr  6 17:41 known_hosts
```

In `ls -l` output, the file size is the number just before the date.

So in this line:

```text
-rwx------. 1 jovyan users   0 Apr  1 19:38 id_ed25519
```

the `0` is the size of `id_ed25519`, measured in bytes.

If `id_ed25519` is `0` bytes, the private key is not usable. That is why SSH reports `error in libcrypto` and GitHub rejects the login.

## How to fix it

1. Run:

```bash
ssh-keygen
```

2. When you see:

```text
Enter file in which to save the key (/home/jovyan/.ssh/id_ed25519):
/home/jovyan/.ssh/id_ed25519 already exists.
Overwrite (y/n)?
```

Type:

```text
y
```

You must type `y` or the broken key will not be replaced.

3. Press `Enter` to accept the default file location.
4. You can leave the passphrase empty if your course instructions say that is okay.

## Check that the new key is valid

Run:

```bash
ls -l ~/.ssh
```

Your `id_ed25519` file should now be much larger than `0` bytes.

You can also test it with:

```bash
ssh-keygen -y -f ~/.ssh/id_ed25519
```

If the key is valid, this should print a public key and should not show a `libcrypto` error.

## Final steps

1. Show your public key:

```bash
cat ~/.ssh/id_ed25519.pub
```

2. Copy that output and add it on GitHub under `Settings` -> `SSH and GPG keys`.
3. Test the connection:

```bash
ssh -T git@github.com
```

4. Retry your original command:

```bash
git clone git@github.com:ucsb-cs5b-s26/lab01-rachit182.git
```

## Summary

The root cause is usually an empty private SSH key file, often shown as `0` bytes in `~/.ssh/id_ed25519`.

The fix is to regenerate the key and make sure you confirm overwrite with `y`.

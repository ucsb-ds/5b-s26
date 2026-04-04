---
title: Key exists, but does not match
permalink: "/git-issues/key-does-not-match"
layout: default
parent: Git Issues
grand_parent: Topics
nav_order: 3
---

# Key exists, but does not match

## If your screen looks like this

```text
identity_sign: private key /home/cgaucho/.ssh/id_ed25519 contents do not match public
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.
```

You might also see this after trying `git clone`, `git pull`, or `git push`.

## What this usually means

Your private key and public key are not a matching pair anymore.

So GitHub rejects the login, even though a key file exists.

## How to fix it

1. Recreate your SSH keys using the lecture notebook steps (`lec02`, or `lec01` if needed). Look for instructions with `ssh-keygen`.
2. Set global Git config again (the commands that set your `user.email` and `user.name`).
3. Copy the correct new public key from `~/.ssh/id_ed25519.pub`.
4. In GitHub, delete the old SSH key and add the new one you just copied.

## Try again

Rerun your previous Git command (for example, `git clone`).

## Reassurance note

This is a common setup issue. You do not need to debug every line. Recreating the key pair and replacing the old GitHub key usually fixes it.

---
title: "Warning: unprotected key file"
permalink: "/git-issues/warning-unprotected-key-file"
layout: default
parent: Git Issues
grand_parent: Topics
nav_order: 2
---

# {{page.title}}

## If your screen looks like this

```text
jovyan@jupyter-phtcon:~/github$ git clone git@github.com:ucsb-cs5b-s26/lab02-pconrad.git 
Cloning into 'lab02-pconrad'...
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@         WARNING: UNPROTECTED PRIVATE KEY FILE!          @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
Permissions 0760 for '/home/jovyan/.ssh/id_ed25519' are too open.
It is required that your private key files are NOT accessible by others.
This private key will be ignored.
Load key "/home/jovyan/.ssh/id_ed25519": bad permissions
git@github.com: Permission denied (publickey).
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
jovyan@jupyter-phtcon:~/github$ 
```

## What this usually means

It means that you have set up a key file, but you need to adjust the "permissions" of the key file.

Unfortunately, by default, Jupyter hub resets the permissions on the key file every time you log in.

There are two ways to fix this: 
1. the "fix it every time you log in" approach
2. the "fix it once and for all" approach

## The "fix it every time you log in" approach

1. Run this command in your terminal:

```bash
chmod 700 ~/.ssh; chmod 700 ~/.ssh/*
```

### What this command does

This sets the permission for the `~/.ssh` directory and all of the files inside it to `700`, which means that the user can read, write and execute the files, 
but no one else can (not users in the same group, and not other users).

That's necessary in order to use the contents of that directory as a public/private key pair.

### After this, try your git command again.

Rerun your `git` command.  It should work now. For example:

```
jovyan@jupyter-phtcon:~/github$ chmod 700 ~/.ssh; chmod 700 ~/.ssh/*
jovyan@jupyter-phtcon:~/github$ git clone git@github.com:ucsb-cs5b-s26/lab02-pconrad.git 
Cloning into 'lab02-pconrad'...
warning: You appear to have cloned an empty repository.
jovyan@jupyter-phtcon:~/github$
```

## The "fix it once and for all" approach

To fix this once and for all, use this command:

```
echo "chmod 700 ~/.ssh; chmod 700 ~/.ssh/*" >> ~/.bashrc
```

### What this does

This sets up a file called `~/.bashrc` if it doesn't already exist, and adds this line of code to the end of the file:

```
chmod 700 ~/.ssh; chmod 700 ~/.ssh/*
```

The left hand side of the command is like a print statement in Python; `echo` is the shell command that corresponds to `print`:

```
echo "chmod 700 ~/.ssh; chmod 700 ~/.ssh/*"
```

The `>>` operator says: whatever the output of this command is (the command on the left hand side), put it at the end of the file on the right hand side (in this case, `~/.bashrc`)

The file `~/.bashrc` is a file of shell commands (terminal commands) that is executed every time you create a new terminal session (shell).

You can use this same approach for anything that you want to be executed once every time you log in.






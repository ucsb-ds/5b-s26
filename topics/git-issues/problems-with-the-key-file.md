---
title: Problems with the key file
permalink: "/git-issues/problems-with-the-key-file"
layout: default
parent: Git Issues
grand_parent: Topics
nav_order: 1
---

# Problems with the key file

## If your screen looks like this

```text
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@ WARNING: UNPROTECTED PRIVATE KEY FILE!                 @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
Permissions 0660 for '/home/cgaucho/.ssh/id_ed25519' are too open.
This private key will be ignored.
bad permissions
Permission denied (publickey).
fatal: Could not read from remote repository.
```

## What this usually means

Your SSH key file permissions are too open, so GitHub refuses to use the key.

This often happens when a key was created in one Jupyter session and then used in a later session.

## How to fix it

1. Run these commands in your terminal:

```bash
chmod 700 ~/.ssh
chmod 700 ~/.ssh/*
```

## Try again

Rerun the same Git command you tried before (for example, your `git clone` or `git push` command).

## Reassurance note

Do not worry about the word ‘fatal’. In this case, it usually just means Git stopped because the key setup needs to be fixed.

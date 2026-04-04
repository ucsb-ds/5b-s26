---
title: Host key verification failed
permalink: "/git-issues/host-key-verification-failed"
layout: default
parent: Git Issues
grand_parent: Topics
nav_order: 2
---

# Host key verification failed

## If your screen looks like this

```text
The authenticity of host 'github.com' can't be established.
ED25519 key fingerprint is SHA256:xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx.
Are you sure you want to continue connecting (yes/no/[fingerprint])?
Host key verification failed.
fatal: Could not read from remote repository.
```

## What this usually means

Your computer has not saved GitHub as a trusted host yet.

Sometimes typing yes interactively does not work properly in Jupyter terminals.

## How to fix it

1. Run this command in your terminal:

```bash
ssh-keyscan github.com >> ~/.ssh/known_hosts
```

## What this command does

This manually adds GitHub to your trusted hosts list.

This fix came up in the class help discussion and solved the issue there.

## Try again

Rerun your `git` command.

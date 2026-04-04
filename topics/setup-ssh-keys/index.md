---
title: "Setting Up SSH Keys for GitHub"
permalink: "/setup-ssh-keys"
layout: default
parent: Topics
nav_order: 4
---

# Setting Up SSH Keys for GitHub

SSH keys let GitHub know it is you, without typing your password every time.

Do this once on each machine you use for class:

- JupyterHub terminal
- your laptop terminal
- a lab machine terminal

Some screenshots below are from JupyterHub, but the same commands work in any terminal.

## When should I do this?

Do this before cloning/pushing course repos.

## Why SSH instead of HTTPS?

- Fewer login prompts
- Works smoothly in JupyterHub and terminal workflows
- Common setup in CS courses and real projects

## Steps

1. Open a terminal.

   ![JupyterHub terminal example]({{ '/topics/setup-ssh-keys/setup-ssh-keys-open-jupyterhub-terminal.png' | relative_url }})

2. Make a key:

   ```bash
   ssh-keygen
   ```

   Press `Enter` for each prompt (file location + passphrase) if you want the default setup.

   ![Running ssh-keygen in terminal]({{ '/topics/setup-ssh-keys/setup-ssh-keys-run-ssh-keygen-command.png' | relative_url }})
   ![ssh-keygen output example]({{ '/topics/setup-ssh-keys/setup-ssh-keys-ssh-keygen-success-output.png' | relative_url }})

3. Check that keys were created:

   ```bash
   ls ~/.ssh
   ```

   You should see at least:

   ```text
   id_ed25519
   id_ed25519.pub
   ```

4. Show your public key:

   ```bash
   cat ~/.ssh/id_ed25519.pub
   ```

   Copy the full line.

5. In GitHub, go to **Settings**.

   ![GitHub profile menu with Settings]({{ '/topics/setup-ssh-keys/setup-ssh-keys-github-profile-settings-menu.png' | relative_url }})

6. Open **SSH and GPG keys**.

   ![GitHub SSH and GPG keys sidebar item]({{ '/topics/setup-ssh-keys/setup-ssh-keys-github-ssh-and-gpg-keys-sidebar.png' | relative_url }})

7. Click **New SSH key** and paste your public key.

   - Title: use something clear like `jupyterhub` or `my-laptop`
   - Key type: `Authentication Key`

   ![GitHub add new SSH key form]({{ '/topics/setup-ssh-keys/setup-ssh-keys-github-add-new-ssh-key-form.png' | relative_url }})


## Quick troubleshooting

- `Permission denied (publickey)`:
  Key was not added to GitHub, or wrong GitHub account is logged in.
- Remote starts with `https://`:
  Switch to SSH remote.
- No `~/.ssh` folder:
  Run `ssh-keygen` first.
- Copied wrong file:
  Copy `id_ed25519.pub`, not `id_ed25519`.

## Important

Never share your private key (`~/.ssh/id_ed25519`).

Only copy/share the public key (`~/.ssh/id_ed25519.pub`).

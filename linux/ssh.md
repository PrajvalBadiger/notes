---
title: SSH
author: Prajval
geometry:
- margin=2cm
- top=2cm
papersize: A4
toc: true
urlcolor: blue
---

\newpage{}

# 1 Enable ssh key based login

## 1.1 ssh-keygen

create a ssh key
```bash
ssh-keygen -t ed25519 -C prajwalbadiger@gmail.com
```

## 1.2 Upload the public key

### Using ssh-copy-id

```bash
ssh-copy-id [user]@[ip-address]

```

### Manually

```bash
# login to the remote machine
ssh [user]@[ip-address]
# create .ssh and authorized_keys files
mkdir -p ~/.ssh && touch ~/.ssh/authorized_keys
# set permissions
chmod 700 ~/.ssh && chmod 600 ~/.ssh/authorized_keys
# copy the public key into the authorized_keys file
scp ~/.ssh/id_ed25519.pub [user]@[ip-address]:~/.ssh/authorized_keys
```

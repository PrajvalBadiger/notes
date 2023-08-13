---
title: Configs
author: Prajval
geometry:
- margin=2cm
- top=2cm
papersize: A4
toc: true
urlcolor: blue
---

\newpage{}


# 1. Neovim as manpager

Export the variable MANPAGER in .profile or .zprofile

```bash
export MANPAGER="/bin/sh -c \"col -b | nvim -c 'set ft=man ts=8 nomod nolist nonu noma' -\""
```

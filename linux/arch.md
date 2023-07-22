---
title: Arch Linux
author: Prajval
geometry:
- margin=2cm
- top=2cm
papersize: A4
toc: true
urlcolor: blue
---

\newpage{}

# 1. DWM

## 1.1 find window class and instance name 

```bash
    xprop | awk '
    /^WM_CLASS/{sub(/.* =/, "instance:"); sub(/,/, "\nclass:"); print}
    /^WM_NAME/{sub(/.* =/, "title:"); print}'
```

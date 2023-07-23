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

## 1.2 Enable dark mode in chrome

- goto [chrome://flags/#enable-force-dark](chrome://flags/#enable-force-dark)
- Select: Enable with simple RBG-based inversion
- Relaunch the browser

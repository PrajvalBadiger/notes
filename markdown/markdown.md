---
title: Markdown
author: Prajval
geometry:
- margin=2cm
- top=2cm
papersize: A4
toc: true
urlcolor: blue
---

\newpage{}

# 1. Mermaid

``` mermaid
stateDiagram
[*] --> First
state First {
    [*] --> second
        second --> fifth
            [*] --> third
            third --> fourth
}

```

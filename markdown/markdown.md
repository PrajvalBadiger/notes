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

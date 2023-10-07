```
sequenceDiagram
    agendador->+contaCorrente: debitar()
    contaCorrente->+agendador: badRequeest (400) -> saldoInsuficiente
    agendador->+comunicador: enviarPush("erro ao debitar")
    agendador->+fila: insereDebito(SeuJoao, VAlor)
```mermaid


```
flowchart LR

A[Hard] -->|Text| B(Round)
B --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

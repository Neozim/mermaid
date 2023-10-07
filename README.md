```
sequenceDiagram
    agendador->+contaCorrente: debitar()
    contaCorrente->+agendador: badRequeest (400) -> saldoInsuficiente
    agendador->+comunicador: enviarPush("erro ao debitar")
    agendador->+fila: insereDebito(SeuJoao, VAlor)
```mermaid

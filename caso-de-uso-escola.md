# Caso de Uso - Escola

```mermaid
flowchart LR
    Aluno["Aluno"]
    Professor["Professor"]
    Secretaria["Secretaria"]

    subgraph SistemaEscolar["Sistema Escolar"]
        UC1((Consultar notas))
        UC2((Ver boletim))
        UC3((Lançar notas))
        UC4((Cadastrar aluno))
    end

    Aluno --> UC1
    Aluno --> UC2
    Professor --> UC3
    Secretaria --> UC4

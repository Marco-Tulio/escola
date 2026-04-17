# Caso de uso da escola

```mermaid
flowchart LR
    Aluno["👤 Aluno"]
    Professor["👤 Professor"]
    Secretaria["👤 Secretaria"]

    subgraph SistemaEscolar["Sistema Escolar"]
        UC1((Consultar notas))
        UC2((Ver boletim))
        UC3((Lançar notas))
        UC4((Cadastrar aluno))
        UC5((Autenticar usuário))
        UC6((Emitir boletim em PDF))
        UC7((Recuperar senha))
    end

    Aluno --> UC1
    Aluno --> UC2
    Professor --> UC3
    Secretaria --> UC4

    UC1 -. "<<include>>" .-> UC5
    UC2 -. "<<include>>" .-> UC5
    UC3 -. "<<include>>" .-> UC5
    UC4 -. "<<include>>" .-> UC5

    UC2 -. "<<extend>>" .-> UC6
    UC5 -. "<<extend>>" .-> UC7


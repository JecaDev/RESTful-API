# RESTful API Java

## Diagrama de Classes

``` mermaid
classDiagram
    class Usuario {
        +string nome
        +Conta conta
        +Feature[] features
        +Cartao cartao
        +Novidade[] novidades
    }

    class Conta {
        +string numero
        +string agencia
        +float saldo
        +float limite
    }

    class Feature {
        +string icone
        +string descricao
    }

    class Cartao {
        +string numero
        +float limite
    }

    class Novidade {
        +string icone
        +string descricao
    }

    Usuario "1" --> "1" Conta
    Usuario "1" --> "*" Feature
    Usuario "1" --> "1" Cartao
    Usuario "1" --> "*" Novidade
    ```

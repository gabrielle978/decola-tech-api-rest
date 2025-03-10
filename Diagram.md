# Decola Tech 2025 - Avanade
### Java RestFul Api

## Diagrama de classes
``` mermaid 
classDiagram
    class User {
        +String name
        +Account account
        +List~Feature~ features
        +Card card
        +List~News~ news
    }

    class Account {
        +String number
        +String agency
        +double limit
        +double balance
    }

    class Feature {
        +String icon
        +String description
    }

    class Card {
        +String number
        +double limit
    }

    class News {
        +String icon
        +String description
    }

    User --> Account
    User --> "0..*" Feature
    User --> Card
    User --> "0..*" News

```

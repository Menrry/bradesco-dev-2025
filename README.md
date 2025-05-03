
# Bootcamp Bradesco - Java Cloud Native
Publicando minha API REST na Nuvem, usando Gradle-Groovy, Spring 3.4.4, Java 21, JSON Editor Online, Gemini ai, Mermaid e Railway.


## Diagrama de Classes

```mermaid
classDiagram
  class User {
    +String name
    +Account account
    +List~Feature~ features
    +Card card
    +List~New~ news
  }
  class Account {
    +String number
    +String agency
    +double balance
    +double limit
  }
  class Feature {
    +String icon
    +String description
  }
  class Card {
    +String number
    +double limit
  }
  class New {
    +String icon
    +String description
  }

  User "1"*--"1" Account 
  User "1"*--"N" Feature 
  User "1"*--"1" Card 
  User "1"*--"N" New 
  ```

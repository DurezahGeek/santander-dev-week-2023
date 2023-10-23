# Santander Dev Week 2023
Java RESTfull Api criada para a santander Dev Week. 

![terraform](https://img.shields.io/badge/-Spring-white?style=for-the-badge&logo=UML&color=ec63a1&logoColor=white)

## Diagrama de Classes 

```mermaid
    classDiagram
    class User {
    - name: string
    - account: Account
    - features: Feature[]
    - card: Card
    - news: News[]
  }

  class Account {
    - number: string
    - agency: string
    - balance: float
    - limit: float
  }

  class Feature {
    - icon: string
    - description: string
  }

  class Card {
    - number: string
    - limit: float
  }

  class News {
    - icon: string
    - description: string
  }

  User "1" *-- "1" Account: has
  User "1" *-- "N" Feature: has many
  User "1" *-- "1" Card: has
  User "1" *-- "N" News: has many
```

# Tecnologias Utilizadas

Neste projeto, estamos usando as seguintes tecnologias:

| Tecnologia         | Versão        | Finalidade                                                            |
|--------------------|---------------|-----------------------------------------------------------------------|
| Java              | 17 (LTS)      | Utilizado para desenvolvimento de aplicativos robustos em Java.     |
| Spring Boot       | 3             | Maximiza a produtividade do desenvolvedor com autoconfiguração.      |
| Spring Data JPA   | -             | Simplifica o acesso a dados e integração com bancos de dados SQL.   |
| OpenAPI (Swagger) | -             | Criação de documentação de API eficaz e fácil de entender.          |
| Railway            | -             | Facilita o deploy e monitoramento de soluções na nuvem, oferecendo diversos bancos de dados como serviço e pipelines de CI/CD. |

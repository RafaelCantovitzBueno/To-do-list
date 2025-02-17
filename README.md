# TODO List API com Spring Boot

Este projeto implementa uma API RESTful para gerenciamento de tarefas (To-Do List), permitindo operações CRUD (Create, Read, Update, Delete) para organização e acompanhamento de atividades.

## Tecnologias Utilizadas

- **Spring Boot** (Framework Java para aplicações web)
- **Spring MVC** (Arquitetura para construção de APIs RESTful)
- **Spring Data JPA** (Integração com banco de dados relacional)
- **SpringDoc OpenAPI 3** (Documentação automática da API)
- **MySQL** (Banco de dados relacional)

## Instalação e Execução

### Pré-requisitos

Certifique-se de ter instalado:
- **Java 17** ou superior
- **Maven**
- **MySQL**

### Passos para instalação

1. Clone o repositório:
   ```sh
   git clone https://github.com/RafaelCantovitzBueno/Todo-list.git
   cd Todo-list
   ```

2. Configure o banco de dados no `application.properties`:
   ```properties
   spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
   spring.datasource.username=seu_usuario
   spring.datasource.password=sua_senha
   spring.jpa.hibernate.ddl-auto=update
   ```

3. Compile e execute o projeto:
   ```sh
   mvn spring-boot:run
   ```

A API estará disponível em `http://localhost:8080/`.

## Endpoints Principais

| Método  | Endpoint  | Descrição |
|---------|----------|-----------|
| `GET`   | `/todos` | Lista todas as tarefas |
| `POST`  | `/todos` | Cria uma nova tarefa |
| `GET`   | `/todos/{id}` | Obtém uma tarefa específica |
| `PUT`   | `/todos/{id}` | Atualiza uma tarefa específica |
| `DELETE` | `/todos/{id}` | Exclui uma tarefa específica |

## Documentação da API

A documentação interativa está disponível via Swagger UI em:
```
http://localhost:8080/swagger-ui.html
```

## Licença

Este projeto está sob a licença MIT. Sinta-se à vontade para usá-lo e modificá-lo conforme necessário.

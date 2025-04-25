# Voll.med API

Este projeto é uma API REST desenvolvida em Java utilizando o framework Spring Boot 3. A API é parte de uma aplicação para gerenciamento de médicos, pacientes e consultas médicas.

## Funcionalidades

- **CRUD de Médicos**: Cadastro, listagem, atualização e exclusão lógica de médicos.
- **CRUD de Pacientes**: Cadastro, listagem, atualização e exclusão lógica de pacientes.
- **Agendamento de Consultas**: Agendamento de consultas médicas com validações de disponibilidade.
- **Autenticação JWT**: Login e autenticação de usuários utilizando tokens JWT.
- **Documentação OpenAPI**: Documentação interativa da API com Swagger.

## Tecnologias Utilizadas

- **Java 21**
- **Spring Boot 3**
- **Spring Security**
- **Spring Data JPA**
- **Flyway** (para controle de migrações de banco de dados)
- **MySQL** (banco de dados relacional)
- **Swagger/OpenAPI** (documentação da API)
- **JUnit 5** e **Mockito** (testes unitários e de integração)

## Estrutura do Projeto

```plaintext
src/
├── main/
│   ├── java/
│   │   └── med/voll/api/
│   │       ├── controller/   # Controladores REST
│   │       ├── domain/       # Entidades, repositórios e serviços
│   │       ├── infra/        # Configurações e infraestrutura
│   └── resources/
│       ├── db/migration/     # Scripts de migração do Flyway
│       ├──   # Configurações da aplicação
├── test/
│   └── java/                 # Testes unitários e de integração
 ```

## Configuração do Ambiente

1. **Pré-requisitos**:
   - Java 21 ou superior
   - Maven
   - MySQL

2. **Configuração do Banco de Dados**:
   - Crie um banco de dados chamado `vollmed_api`.
   - Configure as credenciais no arquivo `src/main/resources/application.properties`.

3. **Executando a Aplicação**:
   - Compile e execute o projeto com o Maven:
     ```bash
     ./mvnw spring-boot:run
     ```

4. **Acessando a API**:
   - A API estará disponível em: `http://localhost:8080`.

5. **Documentação da API**:
   - Acesse a documentação interativa em: `http://localhost:8080/swagger-ui.html`.

## Testes

- Para executar os testes, utilize o comando:
  ```bash
  ./mvnw test
  ```

## Licença

Este projeto está licenciado sob a [Apache License 2.0](http://voll.med/api/licenca).
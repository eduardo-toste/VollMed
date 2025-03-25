# Voll.med - API de Clínica Médica

## Visão Geral
A **Voll.med API** é uma solução robusta para o gerenciamento de clínicas médicas, permitindo a administração eficiente de médicos, pacientes e consultas. Desenvolvida com **Spring Boot**, a API oferece recursos avançados como autenticação segura, paginação, validações de negócio e integração com banco de dados MySQL.

## Tecnologias Utilizadas
- **Java 23** – Linguagem principal
- **Spring Boot** – Framework para desenvolvimento ágil
- **Spring Security** – Implementação de autenticação e autorização
- **JWT (JSON Web Token)** – Controle de acesso seguro
- **MySQL** – Banco de dados relacional
- **JPA/Hibernate** – Mapeamento objeto-relacional (ORM)
- **Flyway** – Gerenciamento de migrações de banco de dados
- **Springdoc OpenAPI** – Documentação automática da API
- **JUnit 5** e **Spring Boot Test** – Testes automatizados
- **Paginação e Ordenação** – Melhoria na performance das consultas

## Recursos e Funcionalidades
- **CRUD completo** para médicos e pacientes
- **Autenticação e autorização** utilizando JWT
- **Agendamento e cancelamento de consultas médicas**
- **Validações avançadas** para garantir regras de negócio
- **Mecanismo de paginação e ordenação** para otimização das respostas da API
- **Documentação interativa** com Swagger (Springdoc OpenAPI)
- **Testes automatizados** para garantir a qualidade do código

## Endpoints

### Médicos
- `POST /medicos` – Cadastra um novo médico
- `GET /medicos` – Lista médicos com paginação e filtros
- `PUT /medicos/{id}` – Atualiza informações de um médico
- `DELETE /medicos/{id}` – Remove um médico do sistema

### Pacientes
- `POST /pacientes` – Cadastra um novo paciente
- `GET /pacientes` – Lista pacientes com paginação e filtros
- `PUT /pacientes/{id}` – Atualiza informações de um paciente
- `DELETE /pacientes/{id}` – Remove um paciente do sistema

### Consultas
- `POST /consultas` – Realiza o agendamento de uma consulta médica
- `DELETE /consultas/{id}` – Permite o cancelamento de uma consulta

### Autenticação
- `POST /auth/login` – Realiza a autenticação do usuário e retorna um token JWT

## Documentação da API
A API é documentada automaticamente utilizando **Springdoc OpenAPI**. Após iniciar a aplicação, acesse a documentação interativa via Swagger:
```declarative
http://localhost:8080/swagger-ui.html
```

### Configuração
1. Defina as credenciais do MySQL no arquivo `application.properties`
2. Execute as migrações do banco com Flyway
3. Inicie a aplicação

### Rodando a Aplicação
```sh
mvn spring-boot:run

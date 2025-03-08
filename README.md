# Voll.med - API de Clínica Médica

API para gerenciamento de médicos e pacientes, desenvolvida com Spring Boot para facilitar o cadastro, consulta, atualização e exclusão de registros.

## Tecnologias
- Java 23
- Spring Boot
- MySQL
- JPA/Hibernate
- Paginação
- Migrations (Flyway)

## Endpoints
### Médicos
- **POST /medicos** - Cadastra um médico
- **GET /medicos** - Lista médicos (com paginação)
- **PUT /medicos** - Atualiza dados de um médico
- **DELETE /medicos/{id}** - Exclui um médico

### Pacientes
- **POST /pacientes** - Cadastra um paciente
- **GET /pacientes** - Lista pacientes (com paginação)
- **PUT /pacientes** - Atualiza dados de um paciente
- **DELETE /pacientes/{id}** - Exclui um paciente

## Configuração
1. Configure o MySQL no `application.properties`
2. Execute as migrations
3. Inicie a aplicação

## Executando
```sh
mvn spring-boot:run
```


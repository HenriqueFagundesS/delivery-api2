# Delivery API

API REST desenvolvida com Spring Boot para um sistema de delivery moderno.

## Tecnologias

- Java 21
- Spring Boot 4.x
- Spring Data JPA
- H2 Database (in-memory)
- Lombok
- Maven

## Como rodar

```bash
mvn spring-boot:run
```

A aplicação sobe na porta `8080`.

## Endpoints

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| GET | `/health` | Status da aplicação |
| GET | `/info` | Informações detalhadas da API |
| GET | `/h2-console` | Console do banco de dados H2 |

### Exemplos

**GET /health**
```json
{
  "status": "FUNCIONANDO !!!",
  "timestamp": "2026-10-15 21:35:00",
  "service": "Delivery API AGOSTO",
  "javaVersion": "21",
  "springBootVersion": "4.11.x",
  "environment": "development"
}
```

**GET /info**
```json
{
  "application": "Delivery Tech API",
  "version": "1.0.0",
  "developer": "Henrique Fagundes Domingos Souza",
  "javaVersion": "21",
  "framework": "Spring Boot 4.11.x",
  "timestamp": "2026-10-15 21:35:00",
  "description": "Sistema de delivery moderno desenvolvido com as mais recentes tecnologias Java"
}
```

## Banco de dados

A aplicação usa H2 in-memory. Para acessar o console:

- URL: `http://localhost:8080/h2-console`
- JDBC URL: `jdbc:h2:mem:deliverydb`
- Usuário: `sa`
- Senha: *(vazio)*

## Desenvolvedor

Henrique Fagundes Domingos Souza

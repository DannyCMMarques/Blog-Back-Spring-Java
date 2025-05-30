# 📖 **PerfectRecipe**

Este é o **MVP** do blog **PerfectRecipe**, uma aplicação CRUD completa de posts para facilitar a criação, edição, exclusão e listagem com paginação de receitas.

---

## 📋 Descrição do Desafio
No contexto de um blog, este desafio consiste no desenvolvimento de uma API REST em Java com Spring Boot para gerenciar posts de receitas via dispositivos móveis e web.

- ✅ **CRUD completo de posts** (Create, Read, Update, Delete)
- ✅ **Paginação** de listagem de posts
- ✅ **Persistência** dos dados mesmo após reinício da aplicação
- ✅ **Pré-população** com 6 posts de exemplo para teste e visualização imediata

---

## 🚀 Tecnologias Utilizadas

- Java 17
- Spring Boot
- Spring Data JPA
- Spring AOP
- Banco de dados H2 / PostgreSQL
- Swagger / OpenAPI
- JUnit 5 e Mockito
- Flyway
- Docker & Docker Compose
- Lombok
- MapStruct

---

## 🏗️ Arquitetura

A aplicação segue uma arquitetura em camadas:

1. **Camada Controller** (`web.rest`): Recebe e responde às requisições HTTP.
2. **Camada Service** (`service`): Contém a lógica de negócio.
3. **Camada Repository** (`repository`): Comunicação com o banco de dados via Spring Data JPA.
4. **DTOs & Mappers** (`service.dto` / `service.mapper`): Separam entidades de domínio e facilitam a troca de dados.
5. **Tratamento de Exceptions** (`exceptions`): Erros específicos com mensagens amigáveis.
6. **Domínio** (`domain`): Entidades principais — Post.
7. **AOP Logging** (`aop.logging`): Logs de entrada, saída e erros.

---

## 🐳 Como Clonar e Rodar o Projeto

```bash
# Clone o repositório
git clone https://github.com/DannyCMMarques/backBlog.git
cd backBlog

# Construa e inicie os containers
docker-compose build
docker-compose up
```

> 🚨 O projeto já vem **pré-populado** com **6 posts** de exemplo para facilitar a visualização e testes de paginação.

---

## 📚 Documentação da API (Swagger)
A documentação interativa está disponível em:

```
http://localhost:8080/swagger-ui.html
```

Certifique-se de que a aplicação esteja executando antes de acessar o link.

---

## 🧪 Testes Automatizados

Para garantir a qualidade, foram implementados testes:

- **Testes de Integração** nos Controllers (MockMvc)
- **Testes Unitários** na camada de Service (Mockito)

### Tecnologias de Teste

- JUnit 5
- Mockito
- Spring Boot Test
- MockMvc

### ▶️ Executar os Testes

```bash
mvn test
```

---

Bom desenvolvimento!

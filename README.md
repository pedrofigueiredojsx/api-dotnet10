# 🚀 API CRUD - C# e .NET 10

Projeto desenvolvido durante os estudos de **C# e .NET 10**, baseado na série [Jornada do Herói](https://www.youtube.com/), apresentada por Henrique Giaretta.

O objetivo do projeto é desenvolver uma API REST utilizando **Minimal APIs**, aplicando conceitos de organização de código, persistência de dados e operações CRUD (Create, Read, Update e Delete).

## 🛠️ Tecnologias utilizadas

- **C#** – Linguagem de programação.
- **.NET 10** – Framework para desenvolvimento da API.
- **ASP.NET Core Minimal APIs** – Construção de endpoints HTTP.
- **Entity Framework Core** – ORM para comunicação com o banco de dados.
- **SQLite** – Banco de dados relacional.
- **Swagger** – Documentação e testes dos endpoints.

## 📌 Funcionalidades

A API permite realizar operações de gerenciamento de pessoas:

| Método | Endpoint       | Descrição                          |
| ------ | -------------- | ---------------------------------- |
| POST   | `/person`      | Cadastra uma nova pessoa.          |
| GET    | `/person`      | Lista as pessoas cadastradas.      |
| PUT    | `/person/{id}` | Atualiza os dados de uma pessoa.   |
| DELETE | `/person/{id}` | Desativa uma pessoa (Soft Delete). |

## 🏗️ Conceitos aplicados

Durante o desenvolvimento, foram trabalhados os seguintes conceitos:

- Criação de APIs REST com Minimal APIs.
- Organização de rotas utilizando Extension Methods.
- Separação de responsabilidades e organização do projeto.
- Criação de modelos utilizando classes e GUID como identificador.
- Utilização de Records para representar objetos de requisição.
- Integração com banco de dados utilizando Entity Framework Core.
- Persistência de dados com SQLite.
- Gerenciamento de migrations.
- Operações assíncronas com `async` e `await`.
- Implementação de Soft Delete.
- Documentação e testes de endpoints com Swagger.

## ⚙️ Como executar o projeto

**1. Clone o repositório**

```bash
git clone https://github.com/SEU-USUARIO/SEU-REPOSITORIO.git
```

**2. Acesse a pasta do projeto**

```bash
cd SEU-REPOSITORIO
```

**3. Restaure as dependências**

```bash
dotnet restore
```

**4. Atualize o banco de dados**

```bash
dotnet ef database update
```

**5. Execute a aplicação**

```bash
dotnet run
```

Após iniciar a aplicação, acesse a URL disponibilizada no terminal para visualizar a documentação Swagger, caso esteja habilitada no ambiente de execução.

## 🎯 Objetivo do projeto

Este projeto faz parte da minha jornada de aprendizado em desenvolvimento Back-end com C#, buscando consolidar conhecimentos na construção de APIs REST, integração com bancos de dados e boas práticas de organização e estruturação de aplicações.

---

**Desenvolvido com 💻 e dedicação aos estudos de C# e .NET.**

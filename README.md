# 🚀 API CRUD - C# e .NET 10

Projeto de estudo de **C# e .NET 10**, feito acompanhando a série **Jornada do Herói**, de Henrique Giaretta: [link da série](COLE-O-LINK-AQUI).

API REST com **Minimal APIs** que pratica organização de código, persistência de dados e operações CRUD.

## 🛠️ Tecnologias

- **C#** e **.NET 10**
- **ASP.NET Core Minimal APIs**
- **Entity Framework Core** (ORM)
- **SQLite** (banco de dados)
- **Swagger** (documentação e testes dos endpoints)

## 📌 Endpoints

| Método | Endpoint       | Descrição                         |
| ------ | -------------- | --------------------------------- |
| POST   | `/person`      | Cadastra uma nova pessoa          |
| GET    | `/person`      | Lista as pessoas cadastradas      |
| PUT    | `/person/{id}` | Atualiza os dados de uma pessoa   |
| DELETE | `/person/{id}` | Desativa uma pessoa (Soft Delete) |

O arquivo `Person.http` tem exemplos de requisição para testar cada endpoint direto no editor.

## 🏗️ Conceitos aplicados

- Minimal APIs com rotas organizadas via Extension Methods
- Models com `GUID` como identificador
- Records para representar os objetos de requisição
- Entity Framework Core com SQLite e migrations
- Operações assíncronas com `async` e `await`
- Soft Delete
- Documentação e testes de endpoints com Swagger

## 📁 Estrutura

```
├── Data/          # Contexto do banco (EF Core)
├── Migrations/    # Migrations do EF Core
├── Models/        # Modelos da aplicação
├── Routes/        # Endpoints (Extension Methods)
├── Properties/    # Configurações de execução
├── Program.cs     # Ponto de entrada
├── Person.http    # Requisições de exemplo
└── Person.csproj
```

## ⚙️ Como executar

Pré-requisito: [.NET 10 SDK](https://dotnet.microsoft.com/download) e a ferramenta do EF Core (`dotnet tool install --global dotnet-ef`).

```bash
git clone https://github.com/pedrofigueiredojsx/api-dotnet10.git
cd api-dotnet10
dotnet restore
dotnet ef database update
dotnet run
```

Acesse a URL exibida no terminal para abrir o Swagger.

## 🎯 Objetivo

Parte da minha jornada de estudos em back-end com C#, consolidando APIs REST, integração com banco de dados e organização de projeto.

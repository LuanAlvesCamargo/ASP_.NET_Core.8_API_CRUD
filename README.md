# ASP.NET Core 8 API CRUD

Este é um projeto de estudo que implementa uma API RESTful utilizando ASP.NET Core 8 Web API e Entity Framework Core 8.

## Funcionalidades

- Permite a realização de operações CRUD (Create, Read, Update, Delete) em dados de filmes.
- Integra serviços de identidade para autenticação e autorização.
- Implementa JSON Web Tokens (JWT) para segurança e controle de acesso.
- Segue as melhores práticas da indústria para escalabilidade e manutenção.

## Tecnologias Utilizadas

- **ASP.NET Core 8** - Framework para desenvolvimento de APIs.
- **Entity Framework Core 8** - ORM para manipulação de banco de dados.
- **JWT (JSON Web Tokens)** - Implementação de segurança e controle de acesso.
- **SQL Server** - Banco de dados relacional utilizado.

## Como Executar o Projeto

### Requisitos

- .NET 8 SDK instalado
- SQL Server configurado

### Passos

1. Clone o repositório:
   ```sh
   git clone https://github.com/LuanAlvesCamargo'/ASP_NET_Core_8_API_CRUD.git
   cd ASP_NET_Core_8_API_CRUD
   ```
2. Configure a string de conexão no `appsettings.json`.
3. Aplique as migrações do banco de dados:
   ```sh
   dotnet ef database update
   ```
4. Execute a aplicação:
   ```sh
   dotnet run
   ```
5. Acesse a API via Swagger em `https://localhost:5001/swagger`.

## Estrutura do Projeto

- `Controllers/` - Contém os controladores da API.
- `Models/` - Contém as classes de modelo do banco de dados.
- `Data/` - Contém o contexto do Entity Framework.
- `Services/` - Implementação de serviços auxiliares.

## Endpoints Principais

| Método | Rota               | Descrição                   |
| ------ | ------------------ | --------------------------- |
| GET    | `/api/movies`      | Lista todos os filmes       |
| GET    | `/api/movies/{id}` | Retorna um filme específico |
| POST   | `/api/movies`      | Adiciona um novo filme      |
| PUT    | `/api/movies/{id}` | Atualiza um filme existente |
| DELETE | `/api/movies/{id}` | Remove um filme             |

## Licença

Este projeto é distribuído sob a Licença MIT. 


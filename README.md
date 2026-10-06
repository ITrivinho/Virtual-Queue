# VirtualQueue

SaaS de fila virtual para lavanderias, com arquitetura multi-tenant planejada para atender várias lavanderias mantendo seus dados isolados.

Projeto em desenvolvimento inicial, construído também como prática de ASP.NET Core e arquitetura web. As regras de negócio e o isolamento entre tenants ainda não foram implementados.

## Tecnologias

- Backend: C# e ASP.NET Core Web API (.NET 10).
- Frontend: React, TypeScript e Vite.
- Testes do backend: xUnit.
- Persistência planejada: PostgreSQL e Entity Framework Core.

## Estrutura

- `backend/VirtualQueue.Api/`: API.
- `backend/VirtualQueue.Api.Tests/`: projeto de testes.
- `frontend/`: aplicação React.
- `docs/`: orientações e documentação do projeto.

## Executar localmente

Requisitos: SDK .NET 10 e Node.js compatível com Vite 8.

Na raiz, inicie a API:

```powershell
dotnet run --project backend/VirtualQueue.Api --launch-profile http
```

A API estará disponível em `http://localhost:5136`.

Em outro terminal, inicie o frontend:

```powershell
cd frontend
npm install
npm run dev
```

Para executar os testes do backend, use `dotnet test` na raiz.

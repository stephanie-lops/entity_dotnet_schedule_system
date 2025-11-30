# DIO - Trilha .NET - API e Entity Framework
www.dio.me

## Desafio de projeto
Neste desafio, apliquei na prática todos os conhecimentos adquiridos no módulo de **API e Entity Framework** da trilha .NET da DIO. O objetivo foi desenvolver uma **API completa para gerenciamento de tarefas**, utilizando **.NET + Entity Framework + SQLite**.

- Desafio finalizado com sucesso  
- Todas as funcionalidades implementadas  
- CRUD completo em funcionamento  
- Migration criada e banco configurado  
- Swagger funcionando corretamente  

## Contexto do Projeto
Desenvolvi um **sistema gerenciador de tarefas**, no qual é possível:

- Cadastrar tarefas
- Listar todas as tarefas
- Filtrar tarefas por:
  - Título  
  - Data  
  - Status  
- Atualizar tarefas
- Excluir tarefas

Toda a aplicação foi construída no formato de **Web API**, utilizando **boas práticas de desenvolvimento**, controle de rotas e persistência com **Entity Framework**.

![Diagrama da classe Tarefa](diagrama.png)

Não se esqueça de gerar a sua migration para atualização no banco de dados.

##  Model da Tarefa

A classe principal do sistema é a **Tarefa**, que possui a seguinte estrutura:

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2025-11-30T10:00:00",
  "status": 0
}
```
Onde o status representa um Enum:
0 → Pendente
1 → Finalizado
2 → Cancelado

## Métodos esperados

**Swagger**


![Métodos Swagger](swagger.png)


**Endpoints**
Todos os endpoints foram implementados e testados via Swagger:

| Verbo  | Endpoint                | Parâmetro | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Tarefa/{id}            | id        | N/A           |
| PUT    | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE | /Tarefa/{id}            | id        | N/A           |
| GET    | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET    | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET    | /Tarefa/ObterPorData    | data      | N/A           |
| GET    | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST   | /Tarefa                 | N/A       | Schema Tarefa |


## Tecnologias Utilizadas

- .NET 9
- Entity Framework Core 8
- SQLite
- Swagger
- API REST
- Migrations
- Git e GitHub

## Status do Projeto
✔ CRUD completo implementado
✔ Banco configurado com SQLite
✔ Migrations aplicadas
✔ Todas as rotas funcionando
✔ Projeto versionado no GitHub

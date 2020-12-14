# Trabalho Individual - GCES - 2020/1

Larissa Siqueira Sales
16/0130883

## Conteinerização

Para a execução do projeto foram criados 3 conteineres:

- github-profile-indexer-client (_Frontend_)
- github-profile-indexer-api (_Backend_)
- db (_Database_)

Para a criação desses conteineres, foram utilizadas as ferramentas **Docker**, na versão 19.03, e **Docker Compose**, na versão 3.7. 

No  diretório `./api`, foram criados os arquivos `dockerfile` (apenas para o _backend_) e `db.env` (para o _database_), enquanto no diretório `./client` foi criado um outro arquivo `dockerfile` (apenas para o _frontend_).

### Execução da aplicação

Para subir a aplicação, basta executar o seguinte comando na raiz do projeto:

```bash
$ docker-compose up
```

A aplicação estará disponível nos seguintes endereços:

- Frontend: `localhost:8080/`
- Backend: `localhost:3000/`


## Integração Contínua

Para configurar o _CI_ do projeto, foi utilizada a ferramenta **GitHub Actions** e para coletar as métricas de qualidade foi utilizada a ferramenta **SonarCloud**.

O _CI_ configurado realiza dois _jobs_:

- client_frontend
- api_backend

Cada job realiza as etapas necessárias para cada camada da aplicação, como instalação de dependências, _build_, execução dos testes e coleta de métricas.

As métricas do projeto podem ser verificadas no [SonarCloud](https://sonarcloud.io/dashboard?id=larissa-sales_Trabalho-Individual-2020-1).

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=larissa-sales_Trabalho-Individual-2020-1&metric=alert_status)](https://sonarcloud.io/dashboard?id=larissa-sales_Trabalho-Individual-2020-1) [![Bugs](https://sonarcloud.io/api/project_badges/measure?project=larissa-sales_Trabalho-Individual-2020-1&metric=bugs)](https://sonarcloud.io/dashboard?id=larissa-sales_Trabalho-Individual-2020-1) [![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=larissa-sales_Trabalho-Individual-2020-1&metric=sqale_rating)](https://sonarcloud.io/dashboard?id=larissa-sales_Trabalho-Individual-2020-1) [![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=larissa-sales_Trabalho-Individual-2020-1&metric=reliability_rating)](https://sonarcloud.io/dashboard?id=larissa-sales_Trabalho-Individual-2020-1) [![Lines of Code](https://sonarcloud.io/api/project_badges/measure?project=larissa-sales_Trabalho-Individual-2020-1&metric=ncloc)](https://sonarcloud.io/dashboard?id=larissa-sales_Trabalho-Individual-2020-1) 


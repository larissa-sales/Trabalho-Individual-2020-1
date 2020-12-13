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
- Backeend: `localhost:3000/`
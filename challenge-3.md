## Desafio

### Problema

Pra finalizar essa etapa, crie o comando pra criar o banco de dados MongoDB usando os requisitos abaixo:

- O usuário root do banco deve ser `mongo_usr`
- A senha do usuário root deve ser `mongo_pwd`

Lembrando que a execução em container deve ser transparente pra quem está desenvolvendo. E que aqui você não precisa se preocupar com a perda dos dados do banco e nem nada disso, é apenas para desenvolvimento pontual.

### Solução

```bash
docker run --name mongo_dev -e MONGO_INITDB_ROOT_USERNAME=mongo_usr -e MONGO_INITDB_ROOT_PASSWORD=mongo_pwd -p 27017:27017 -d mongo
```

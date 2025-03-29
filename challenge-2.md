## Desafio

### Problema

Agora que a equipe tem como criar o banco de dados Postgre, crie o comando pra criar o banco de dados MySQL usando os requisitos abaixo:

- O nome do banco de dados deve ser `docker_db`
- O usuário de acesso ao banco deve ser `docker_usr`
- A senha do usuário deve ser `docker_pwd`

Lembrando que a execução em container deve ser transparente pra quem está desenvolvendo. E que aqui você não precisa se preocupar com a perda dos dados do banco e nem nada disso, é apenas para desenvolvimento pontual.

### Solução

```bash
docker run --name mysql_dev -e MYSQL_DATABASE=docker_db -e MYSQL_USER=docker_usr -e MYSQL_PASSWORD=docker_pwd -e MYSQL_ROOT_PASSWORD=root -p 3306:3306 -d mysql
```

# Tela Segura

## O projeto serve para demonstrar a tela de login segura. Usado para testar quando um usuário está logado e aceitar apenas uma conexão por vez.
<br>

# Como funciona

### Primeiro devemos baixar ou clonar o repositório.

```bash

$ git clone https://github.com/mmespido/tela-segura.git
```

### Depois, devemos executar o comando de criar a base de dados, nesse caso, foi utilizado a database "telaSegura".

```bash

$ CREATE DATABASE telaSegura;

```

### Então é criado a tabela "users", ela é a única necessária no projeto.

```bash

$ CREATE TABLE users(
    id INT PRIMARY KEY AUTO_INCREMENT,
    username VARCHAR(45) NOT NULL,
    password VARCHAR(60) NOT NULL,
    created_at VARCHAR(45) NOT NULL,
    user_active BOOLEAN NOT NULL DEFAULT FALSE
);

```

### É necessário renomear o arquivo env para conectar no servidor.

```bash
PORT= [Porta do servidor]
MYSQL_HOST= [Nome do host, por padrão é 'localhost']
MYSQL_USER= [Nome do usuário, utilizado root por padrão]
MYSQL_PASSWORD= [Senha do user, root por padrão também]
MYSQL_DB= [Nome da base de dados, telaSegura nesse caso]
```

### É necessário utilizar os node_modules, para isso o comando abaixo é necessário.

```bash

$ npm install
```

### Então para iniciar o servidor, o comando abaixo é usado (dentro da pasta backend). Depois é só abrir o Index.html.

```bash

$ npm start
```

<br>

# Créditos

- <a href="https://www.youtube.com/@ManualdoDev"> Projeto Todolist React e Docker do Manual do Dev
- <a href="https://www.youtube.com/@will_dev"> Projeto Sistema de Login com React do Will Dev
- <a href="https://www.youtube.com/@bitloop"> Projeto Tela Login do bit loop
- <a href="https://www.youtube.com/@RogerMelo"> Dicas gerais de Javascript, http entre outros assuntos
- <a href="https://www.mysql.com/"> Banco de dados Mysql utilizado
- <a href="https://chat.openai.com/"> Chat GPT 3.5 para consultar dicas e boas práticas de desenvolvimento
- <a href="https://www.docker.com/"> Utilizado docker para subir o banco de dados
- <a href="https://react.dev/"> Feito com React
- <a href="https://nodejs.org/en"> E também feito com Node
- <a href="https://expressjs.com/pt-br/"> E o framework Express.js




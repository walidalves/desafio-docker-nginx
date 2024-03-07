# Desafio Full Cycle

<h2>Utilização do nginx como proxy reverso.</h2>
-> A idéia principal é que quando um usuário acesse o nginx, o mesmo fará uma chamada em nossa aplicação node.js.
-> Essa aplicação por sua vez adicionará um registro em nosso banco de dados mysql, cadastrando um nome na tabela people.

O retorno da aplicação node.js para o nginx deverá ser:

<h2> Full Cycle Rocks!</h2>

Lista de nomes cadastrada no banco de dados.
Gere o docker-compose de uma forma que basta apenas rodarmos: docker-compose up -d que tudo deverá estar funcionando e disponível na porta: 8080.

🌱 Como executar o projeto:

-> Primeiro você deve criar uma network para que os containers possam se comunicar entre si:
   docker network create app-node-network

-> Executar o comando docker-compose para subir os containers:
docker-compose up -d

-> Acessar a aplicação em seu browser:
http://localhost:8080

-> Para aparecer um novo nome, precisa atualizar a página para adicionar ao banco de dados.

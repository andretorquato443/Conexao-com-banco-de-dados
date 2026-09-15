Este programa é uma aplicação console desenvolvida em Java que se conecta a um banco de dados relacional Postgres rodando em container Docker para gerenciar e consultar os dados de uma plataforma fictícia de streaming no estilo Netflix, permitindo interagir via terminal através de um menu  para rodar consultas SQL complexas e exibir dados das entidades da tabela de forma organizada.
É necessario ter Java JDK 17+ , Postgres SQL e Docker

Como configurar o Postgres:

1-Crie o banco de dados PostgreSQL com o nome: "netflix"

2-Execute tabelas.sql

3-Execute o arquivo instancias.sql (para popular os dados de teste)


Como rodar :

1-clona o repositório :git clone https://github.com/andretorquato443/Conexao-com-banco-de-dados.git
cd Conexao-com-banco-de-dados

2-altera em Conexoes.java os atributos usuario e senha para os valores de seu usuario e senha do seu postgres(para o programa em java se conectar ao seu postgres local)

3- execute este comando no terminal : docker run --name postgres-netflix -e POSTGRES_PASSWORD=postgres -e POSTGRES_DB=netflix -p 5432:5432 -d postgres

4-pode dar run na main 



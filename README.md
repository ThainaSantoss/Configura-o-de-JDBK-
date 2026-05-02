# Configuração de JDBC


Usando MySQL para configuração de projeto Java com JDBC para sincronizar projeto de exemplo. Este codigo foi feito com intuito apenas de mostrar conexão com banco de dados MySQL.


## Ferramentas utilizadas

- Java  
- JDBC  
- MySQL  
- MySQL Workbench  
- Git/GitHub

## Configuração de banco de dados

A criação foi feita de forma simples apenas para montagem de projeto

- Crie um banco de dados no MySQL

    CREATE DATABASE IF NOT EXISTS coursejdbc;

- Crie um usuário de aplicação 

    CREATE USER IF NOT EXISTS 'dev'@'localhost' IDENTIFIED BY 'sua_senha';

- Conceda permissão ao usuário no banco:

    GRANT  ALL  PRIVILEGES  ON coursejdbc.*  TO  'dev'@'localhost';  
    FLUSH PRIVILEGES;

## Observações

- O projetinho utiliza um arquivo `db.properties` para armazenar os dados de conexão com o banco.
- Crie um arquivo chamado `db.properties` na raiz do projeto;
- O arquivo `db.example.properties` serve apenas como exemplo de configuração.



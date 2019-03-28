# Node_htttp
API Restfull Node para pagamentos.  
 
## Payfast  
Projeto da API  
 
## Cardfast  
Cliente Node para testes e consumo da API  

## Instalação e configuração do banco

### Instalando o MySql

[Instalando MySql (Alura)](https://cursos.alura.com.br/course/introducao-a-banco-de-dados-e-sql/task/5652)  
[Corrigindo possíveis problemas](https://cursos.alura.com.br/forum/topico-erro-er_not_supported_auth_mode-client-does-not-support-authentication-protocol-requested-by-server-consider-upgrading-mysql-client-61991)

### Criando as tabelas necessárias

com o terminal/cmd aberto:

> mysql -u root  

> create database payfast;
  
> use payfast;
  
> CREATE TABLE pagamentos (id int(11) NOT NULL AUTO_INCREMENT, forma_de_pagamento varchar(255) NOT NULL, valor decimal(10,2) NOT NULL, moeda varchar(3) NOT NULL, status varchar(255) NOT NULL, data DATE, descricao text, PRIMARY KEY (id));  

## Configuração dos módulos do Node
caso algum módulo não esteja configurado corretamente

> cd casadocodigo  
> npm install  
> npm install -g nodemon

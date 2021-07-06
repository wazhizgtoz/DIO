# Conceitos de  melhores práticas  com  bancos de dados PostgreSQL



Este curso ensinará como trabalhar com PostgreSQL, um  gerenciador de banco de dados relacional.



###  Anotações

_Anotações importantes do  curso_

Quando tentei acessar o banco com o usuário **postgres**  solicitou uma senha.  No Ubuntu  tentei  o comando  abaixo:

**$**  _sudo su  - postgres_ 		// Usuário dono do processo



**$** _psql_									// Conectando ao banco



CREATE ROLE administradores
CREATEDB
CREATEROLE
INHERIT
NOLOGIN
REPLICATION
BYPASSRLS
CONNECTION LIMIT -1;

CREATE ROLE  gerente
NOCREATEDB
NOLOGIN
INHERIT
NOCREATEROLE
NOBYPASSRLS
CONNECTION LIMIT 90;

CREATE ROLE cliente
NOCREATEDB
NOCREATEROLE
INHERIT
NOLOGIN
NOBYPASSRLS
CONNECTION LIMIT 90;


CREATE ROLE bootcampLOGIN CONNECTION LIMIT 1  PASSWORD '123' IN ROLE administradores;




###  Concluído?

- [ ] sim
- [ ] não

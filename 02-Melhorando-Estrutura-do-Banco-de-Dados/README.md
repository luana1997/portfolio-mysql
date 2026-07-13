#Aula 04 - Criando a primeira tabela

##🎯 Objetivo

Aprender a criar tabelas no MySQL, definir tipos de dados, configurar chaves primárias e utilizar valores padrão.

##📚 Comandos utilizados
CREATE DATABASE
USE
CREATE TABLE
PRIMARY KEY
AUTO_INCREMENT
VARCHAR
DATE
ENUM
DECIMAL
DEFAULT
CHARACTER SET

##💻 Script SQL

```sql
create database cadastro
default character set utf8mb3
default collate utf8_general_ci;

use cadastro;

Create table pessoas (
id int not null auto_increment,
nome varchar (30) not null,
nascimento date,
sexo enum ('M' , 'F'),
peso decimal (5,2),
altura decimal (3,2),
nacionalidade varchar (20) default 'Brasil',
primary key (id)
) default charset = utf8mb4;
```

## ✅ Resultado
- Banco de dados criado com sucesso.
- Tabela pessoas criada.
- Chave primária configurada.
- Identificador automático funcionando.
- Valor padrão definido para a nacionalidade.

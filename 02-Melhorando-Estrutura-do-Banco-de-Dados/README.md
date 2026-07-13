# Aula 02 - Criando a primeira tabela

## 🎯 Objetivo
Aprender a criar tabelas no MySQL, definir tipos de dados, configurar chaves primárias e utilizar valores padrão.

## 📚 Comandos utilizados
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

## 💻 Script SQL

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

  <img width="736" height="519" alt="Captura de tela 2026-07-13 133314" src="https://github.com/user-attachments/assets/a9729fe3-79ea-4296-8f0a-f48e8ddc34c1" />

  ## 📖 O que aprendi
  
- Criar uma tabela no MySQL utilizando o comando `CREATE TABLE`.
- Definir diferentes tipos de dados para cada coluna (`INT, VARCHAR, DATE, ENUM e DECIMAL`).
- Configurar uma chave primária com `PRIMARY KEY`.
- Utilizar `AUTO_INCREMENT` para gerar identificadores automaticamente.
- Definir valores padrão com a cláusula `DEFAULT`.


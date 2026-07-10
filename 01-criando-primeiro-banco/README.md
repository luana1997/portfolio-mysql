# Aula 01 - Criando o primeiro banco de dados

## 🎯 Objetivo

Aprender a criar um banco de dados e a primeira tabela utilizando MySQL.

## 📚 Comandos utilizados

- CREATE DATABASE
- USE
- CREATE TABLE
- DESCRIBE

## ✅ Resultado

A tabela **Pessoas** foi criada com sucesso.

## 💻 Script SQL

```sql
create database Cadastros_de_Pessoas;
use Cadastros_De_Pessoas;
create table Pessoas (
Nome varchar(30),
Idade tinyint(3),
Sexo char (1),
Peso float,
Altura float,
Nacionalidade varchar (20)
);

Describe Pessoas;
````
<img width="789" height="789" alt="Captura de tela 2026-07-10 191235" src="https://github.com/user-attachments/assets/4d9032f0-f623-4d89-8540-7e4d07109a43" />


## 📖 O que aprendi

- Criar um banco de dados.
- Selecionar um banco de dados com o comando `USE`.
- Criar uma tabela utilizando `CREATE TABLE`.
- Conhecer os principais tipos de dados do MySQL.
- Visualizar a estrutura da tabela com `DESCRIBE`.



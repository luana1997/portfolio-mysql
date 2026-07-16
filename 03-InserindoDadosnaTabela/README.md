# Aula 03 - Inserindo Dados na Tabela

## 🎯 Objetivo

Aprender a inserir registros em uma tabela utilizando o comando `INSERT INTO`, adicionando informações de forma manual para o preenchimento dos dados.

## 📚 Comandos utilizados
- INSERT INTO
- VALUES
- Inserção de um único registro
- Inserção de vários registros em um único comando

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

insert into pessoas 
(id, nome, nascimento, sexo, peso, altura, nacionalidade)
values
(default,'Oliver','1979-02-18', 'M', '62.8','1.55', 'USA'),
(default,'Otavio','1989-01-28', 'M', '82.8','1.75', default),
(default,'Olivia','1969-04-08', 'F', '52.8','1.45', 'Africa'),
(default,'Mariana','1999-03-15', 'F', '60.8','1.85', 'Portugal');

select * from pessoas;
```

## ✅ Resultado
- Inserção de registros utilizando o comando `INSERT INTO`.
- Utilização da cláusula `VALUES` para adicionar informações à tabela.
- Inclusão de um ou mais registros em uma única instrução SQL.
- Compreensão da importância de informar as colunas para tornar o código mais seguro e organizado.
- Dados armazenados com sucesso na tabela `pessoas`.
<img width="874" height="808" alt="Captura de tela 2026-07-15 132922" src="https://github.com/user-attachments/assets/31a9457a-41e3-4760-8ff4-94b3bc00c09d" />

 ## 📖 O que aprendi

- Utilizar o comando `INSERT INTO` para inserir registros em uma tabela.
- Informar as colunas da tabela para tornar a inserção de dados mais segura e organizada.
- Utilizar a cláusula `VALUES` para definir os valores que serão inseridos.
- Inserir um único registro ou vários registros em uma única instrução SQL.


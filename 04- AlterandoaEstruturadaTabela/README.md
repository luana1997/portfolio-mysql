# Aula 04 - Alterando a Estrutura da Tabela

## 🎯 Objetivo

Aprender a modificar a estrutura de tabelas já existentes utilizando o comando ALTER TABLE, adicionando, alterando, renomeando e removendo colunas.

## 📚 Comandos utilizados
- ALTER TABLE
- ADD COLUMN
- DROP COLUMN
- MODIFY COLUMN
- CHANGE COLUMN
- RENAME TABLE
- DROP TABLE

## 💻 Script SQL

```sql
create table if not exists Cursos (
Nome varchar (30) not null unique,
Descricao text,
Carga int unsigned,
TotalAulas int,
Ano year default '2016'
) default charset = utf8mb4;

select * from Cursos;

desc Cursos;

alter table Cursos
add column Idcurso int first;

alter table Cursos
add primary key (Idcurso);
```
## ✅ Resultado
- Modifiquei a estrutura de tabelas utilizando o comando ALTER TABLE.
- Adicionei, alterei, renomeei e removi colunas.
- Aprendi a renomear tabelas existentes.
- Entendi quando utilizar o comando DROP TABLE para excluir uma tabela.

## 📖 O que aprendi

- Aprendi a utilizar o comando `ALTER TABLE` para modificar a estrutura de tabelas já existentes.
- Entendi como adicionar novas colunas utilizando `ADD COLUMN`.
- Aprendi a alterar o tipo de dados e outras características de uma coluna com `MODIFY COLUMN`.
- Compreendi como renomear colunas utilizando `CHANGE COLUMN`.
- Aprendi a remover colunas que não são mais necessárias com `DROP COLUMN`.
- Entendi como renomear uma tabela utilizando `RENAME TO`.
- Aprendi que o comando `DROP TABLE` exclui permanentemente uma tabela e todos os seus registros.
- Compreendi a importância desses comandos para realizar a manutenção e evolução de bancos de dados sem precisar recriar tabelas.

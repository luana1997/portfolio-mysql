# Aula 05 - Manipulando Linhas

## 🎯 Objetivo

Aprender a manipular registros em uma tabela utilizando o comando `UPDATE`, realizando alterações em um ou mais campos de uma linha específica e entender o uso de `WHERE` e `LIMIT` para evitar modificações indesejadas.

## 📚 Comandos utilizados

- `USE`
- `SELECT`
- `UPDATE`
- `SET`
- `WHERE`
- `LIMIT`

## ✅ Resultados

- Revisei os conceitos de registros (linhas/tuplas) e campos (colunas).
- Inseri registros na tabela `cursos` para realizar os testes de atualização.
- Atualizei um único campo de um registro utilizando `UPDATE`.
- Modifiquei vários campos de um mesmo registro em uma única instrução.
- Utilizei o comando `WHERE` para identificar qual registro deveria ser alterado.

## 📖 O que aprendi

- Compreendi a diferença entre **registros (linhas ou tuplas)** e **campos (colunas)** em uma tabela.
- Aprendi que o comando `UPDATE` é utilizado para alterar dados já existentes em um banco de dados.
- Utilizei o comando `SET` para definir os novos valores de um ou mais campos de um registro.
- Aprendi que utilizar a **chave primária** na cláusula `WHERE` garante que apenas um registro seja alterado.
- Aprendi que é possível atualizar vários campos de um mesmo registro em um único comando `UPDATE`.
- Aprendi a utilizar `LIMIT` para restringir a quantidade de registros afetados.
- Entendi os riscos de executar um `UPDATE` sem utilizar corretamente o comando `WHERE`.
- Conheci o recurso **Safe Updates** do MySQL Workbench, utilizado para evitar alterações acidentais em múltiplos registros.



# Aula 10 - Select (Parte 2)

## 🎯 Objetivo

Aprofundar o uso do comando SELECT, aprendendo a realizar buscas com padrões usando LIKE, filtrar resultados por partes do texto, utilizar caracteres coringa (% e _), eliminar valores repetidos com DISTINCT e aplicar funções de agregação para contar, somar, calcular médias e encontrar valores máximos e mínimos em uma tabela.

## 📚 Comandos utilizados

- SELECT * FROM cursos;
- SELECT * FROM cursos WHERE nome = 'PHP';
- SELECT * FROM cursos WHERE nome LIKE 'P%';
- SELECT * FROM cursos WHERE nome LIKE '%A';
- SELECT * FROM cursos WHERE nome LIKE '%A%';
- SELECT * FROM cursos WHERE nome NOT LIKE '%A%';
- SELECT * FROM cursos WHERE nome LIKE 'PH%P';
- SELECT * FROM cursos WHERE nome LIKE 'PH%P_';
- SELECT * FROM gafanhotos WHERE nome LIKE '%Silva%';
- SELECT DISTINCT nacionalidade FROM gafanhotos ORDER BY nacionalidade;
- SELECT DISTINCT carga FROM cursos ORDER BY carga;
- SELECT COUNT(*) FROM cursos;
- SELECT COUNT(*) FROM cursos WHERE carga > 40;
- SELECT MAX(carga) FROM cursos;
- SELECT MAX(totaulas) FROM cursos WHERE ano = '2016';
- SELECT MIN(totaulas) FROM cursos WHERE ano = '2016';
- SELECT SUM(totaulas) FROM cursos WHERE ano = '2016';
- SELECT AVG(totaulas) FROM cursos WHERE ano = '2016';

## ✅ Resultado

- Realizar buscas por nomes que começam, terminam ou contêm determinados caracteres.
- Filtrar registros utilizando LIKE e NOT LIKE.
- Listar apenas valores únicos de colunas usando DISTINCT.
- Contar registros com COUNT.
- Identificar maiores e menores valores com MAX e MIN.
- Somar valores com SUM.
- Calcular médias com AVG.

## 📚 O que eu aprendi

- O LIKE é um operador de comparação por semelhança.
- % substitui nenhum, um ou vários caracteres.
- _ substitui exatamente um caractere.
- DISTINCT remove valores repetidos de uma consulta.
- É possível usar WHERE junto com funções de agregação para analisar apenas parte dos dados.
- O comando SELECT é extremamente flexível e pode ser usado tanto para listagens simples quanto para análises de dados mais avançadas.

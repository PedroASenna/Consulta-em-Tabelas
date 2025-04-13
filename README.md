# 🎬 Pagila SQL Queries Project

Este repositório contém consultas SQL desenvolvidas com base no banco de dados **Pagila**, uma versão adaptada do famoso banco de exemplo Sakila para o PostgreSQL. O projeto utiliza o **pgAdmin4** como ferramenta para executar e testar as queries.

## 📂 Estrutura do Projeto

- `pagila-schema.sql` – Script com a estrutura das tabelas do banco.
- `pagila-insert-data.sql` – Script com os dados de inserção.
- `pagila-data.sql` – Script completo para criação e popular o banco.
- `queries.sql` – Arquivo com todas as consultas SQL realizadas no projeto.

## 🧠 Consultas Realizadas

### 1️⃣ 10 filmes com mais de 2h de duração
Lista os **10 filmes mais longos** com duração superior a 120 minutos, ordenados de forma decrescente por duração.

```sql
SELECT title, length
FROM film
WHERE length > 120
ORDER BY length DESC
LIMIT 10;

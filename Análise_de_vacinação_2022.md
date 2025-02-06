
# 📊 Análise de Dados com SQL e Tableau

> Este projeto utiliza SQL para análise de dados e Tableau para visualização interativa.

## 🔍 Descrição do Projeto
O objetivo deste projeto é explorar um conjunto de dados sobre uma vacinação realizado no ano de 2022, em alguns distritos do Estados Unidos.

## 🛠️ Ferramentas Utilizadas
- **SQL**: PostgreSQL para extração dos dados.
- **Tableau**: Para criação dos dashboards. 

## 📂 Estrutura do Projeto
📁 [Análise_de_Vacinação_2022](https://github.com/viniwallaz/Flu_shot_Healthcare/tree/main) │-- 📜 [Instruções.md](https://github.com/viniwallaz/Flu_shot_Healthcare/blob/main/README.md) │-- 📊 [Dashboard.png](https://github.com/viniwallaz/Flu_shot_Healthcare/blob/main/capa_flu_shot_dash.png) │-- 📂 [SQL-queries](https://github.com/viniwallaz/Flu_shot_Healthcare/blob/main/Flu_shot_SQL_final_script.sql) │ -- 📂 [Dataset_utilizado](https://github.com/viniwallaz/Flu_shot_Healthcare/blob/main/Flu%20Demo%20Data%20(1).csv)

## 🏗️ Passo a Passo da Análise

### 1️⃣ Coleta de Dados
Os dados foram extraídos desse repositório e link respectivamente: [Data_Wizardry_github](https://github.com/Data-Wizardry) ; [Flu_Shot_Healthcare_files](https://datawizardry.academy/flu-shot-dashboard/)

### 2️⃣ Consultas SQL Utilizadas
#### 🔹 Exemplo de Query para Filtrar Vendas por Categoria:
```sql
SELECT categoria, SUM(valor_venda) AS total_vendas
FROM vendas
GROUP BY categoria
ORDER BY total_vendas DESC;

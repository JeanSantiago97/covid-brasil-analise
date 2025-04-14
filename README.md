# 📊 covid-brasil-analise

Este repositório contém uma análise detalhada da pandemia de COVID-19 no Brasil, com foco na avaliação proporcional do impacto da doença em diferentes municípios e estados. O estudo leva em consideração dados populacionais e epidemiológicos, permitindo a criação de indicadores derivados como taxa de mortalidade, incidência proporcional, percentual de contaminação e letalidade.

> **Trabalho prático para a disciplina Infraestrutura Google BigQuery do curso de Pós-graduação em Engenharia de Dados (MIT) do Instituto Infnet.**

---

## 🎓 Projeto Acadêmico

**Curso:** Pós-graduação em Engenharia de Dados – MIT  
**Instituição:** Instituto Infnet  
**Disciplina:** Infraestrutura com Google BigQuery  
**Tema:** Processamento e análise de dados com ferramentas do ecossistema GCP

---

## 🛠️ Tecnologias Utilizadas

- **Google BigQuery** – processamento em larga escala e integração com dados públicos
- **Google Colab** – ambiente de desenvolvimento para análise e visualização de dados
- **Python (Pandas, Matplotlib, Seaborn)** – manipulação de dados e geração de gráficos
- **Google Cloud Storage** – armazenamento dos arquivos exportados e integração com BigQuery

---

## 📚 Fonte dos Dados

Os dados utilizados neste projeto foram extraídos do repositório público no Kaggle:

🔗 [Corona Virus Brazil - Kaggle Dataset](https://www.kaggle.com/datasets/unanimad/corona-virus-brazil)

---

## 🔍 Objetivos da Análise

- Identificar os estados com maiores taxas proporcionais de mortalidade por COVID-19
- Verificar a correlação entre densidade populacional e percentual de contaminação
- Avaliar o impacto proporcional da pandemia em municípios pequenos e grandes
- Criar e analisar os seguintes indicadores derivados:
  - `taxa_mortalidade_10k` e `taxa_mortalidade_100k`
  - `incidencia_100k`
  - `letalidade_percentual`
  - `densidade_casos_por_habitante`
  - `percentual_contaminados`
  - `percentual_mortes_populacao`

---

## 📈 Visualizações

O notebook contém os seguintes gráficos:

- **Gráfico de Barras:** Top 10 estados com maior taxa de mortalidade proporcional
- **Gráfico de Dispersão:** Relação entre densidade de casos por habitante e percentual de contaminados
- **Gráfico de Linha (temporal):** Evolução mensal de casos e óbitos em grandes cidades
- **Gráfico de Linha (letalidade):** Comparação da letalidade ao longo do tempo nos estados com maior média

---

## 📁 Estrutura de Arquivos

```
covid-brasil-analise/ 
│ ├── Analise_COVID.ipynb # Notebook com visualizações e análises 
├── tbl_resultado_covid.csv # Base consolidada exportada do BigQuery 
├── README.md # Este arquivo 
├── files/ 
│ ├── ❌ brazil_covid19_cities.csv # Base bruta de casos e óbitos por cidade 
│ ├── ❌ brazil_population_2019.csv # População estimada por cidade em 2019 
│ └── query.txt # Consulta SQL utilizada no BigQuery
```
---

## ✍️ Autor

**Jean Santiago**  
Aluno da Pós-graduação em Engenharia de Dados – Instituto Infnet  
Repositório acadêmico para a disciplina de BigQuery – Abril/2025
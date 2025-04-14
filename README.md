# 📊 covid-brasil-analise

Este repositório contém uma análise detalhada da pandemia de COVID-19 no Brasil, com foco na avaliação proporcional do impacto da doença em diferentes municípios e estados. O estudo leva em consideração dados populacionais e epidemiológicos, permitindo a criação de indicadores derivados como taxa de mortalidade, incidência proporcional, percentual de contaminação e letalidade.

> **Trabalho prático para a disciplina Infraestrutura Google BigQuery do curso de Pós-graduação em Engenharia de Dados (MIT) do Instituto Infnet.**

---

## 📑 Sumário

- [🎓 Projeto Acadêmico](#-projeto-acadêmico)
- [🛠️ Tecnologias Utilizadas](#️-tecnologias-utilizadas)
- [📚 Fonte dos Dados](#-fonte-dos-dados)
- [🔍 Objetivos da Análise](#-objetivos-da-análise)
- [🧠 Perguntas de Análise e Hipótese](#-perguntas-de-análise-e-hipótese)
- [📈 Visualizações](#-visualizações)
- [✅ Análise Final (Resultados)](#-análise-final-resultados)
- [📁 Estrutura de Arquivos](#-estrutura-de-arquivos)
- [✍️ Autor](#️-autor)

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

## 🧠 Perguntas de Análise e Hipótese

### 📌 Perguntas de Investigação

Durante a construção da análise, foram formuladas as seguintes perguntas para guiar a exploração dos dados e avaliar os impactos da pandemia no Brasil:

1. **Quais estados brasileiros apresentaram as maiores taxas proporcionais de mortalidade por COVID-19 em relação à população estimada?**
2. **Existe uma relação entre a densidade de casos por habitante e o percentual de contaminação nas cidades brasileiras?**
3. **Cidades com menor população tiveram, proporcionalmente, maiores taxas de impacto da pandemia?**

### 💡 Hipótese

> Cidades com maior população tenderiam a apresentar maiores números absolutos de casos de COVID-19. Entretanto, cidades de menor porte poderiam registrar taxas proporcionalmente mais elevadas de contaminação e mortalidade, devido a fatores como infraestrutura de saúde limitada, menor capacidade hospitalar ou dificuldade de acesso a políticas públicas. Também se esperava identificar uma correlação entre a densidade de casos e o percentual da população infectada.

---

## 📈 Visualizações

O notebook contém os seguintes gráficos:

- 📊 **Gráfico de Barras:** Top 10 estados com maior taxa de mortalidade proporcional
- 📈 **Gráfico de Dispersão:** Relação entre densidade de casos por habitante e percentual de contaminados
- 📉 **Gráfico de Linha (temporal):** Evolução mensal de casos e óbitos em grandes cidades (ex: Rio de Janeiro, São Paulo)
- 📉 **Gráfico de Linha (letalidade):** Comparação da letalidade ao longo do tempo nos estados com maior média

---

## ✅ Análise Final (Resultados)

A partir da análise dos dados da pandemia no Brasil, foi possível responder às perguntas propostas e confirmar, em grande parte, a hipótese formulada:

1. **Maiores taxas proporcionais de mortalidade** foram registradas nos estados do **Distrito Federal (DF)**, **Mato Grosso (MT)**, **Rondônia (RO)**, **Espírito Santo (ES)** e **Goiás (GO)**, conforme mostrado no gráfico de barras com ajuste por 100 mil habitantes. Isso reforça que o impacto deve ser analisado de forma proporcional à população, e não apenas por números absolutos.

2. **Relação entre densidade de casos e percentual contaminado**: o gráfico de dispersão evidenciou uma forte correlação linear entre a densidade de casos por habitante e o percentual da população infectada, confirmando a expectativa de proporcionalidade entre as variáveis.

3. **Impacto em cidades menores**: diversas cidades com pequena população apresentaram taxas de contaminação e mortalidade significativamente altas, proporcionalmente. Esse resultado confirma que, apesar dos menores números absolutos, o impacto da pandemia pode ser mais severo em municípios com menos infraestrutura.

Essas conclusões demonstram a importância de considerar indicadores normalizados e análises proporcionais ao estudar fenômenos epidemiológicos, promovendo decisões mais justas e eficazes em políticas públicas de saúde.

---

## 📁 Estrutura de Arquivos

- `covid-brasil-analise/`
  - `Analise_COVID.ipynb` – Notebook com visualizações e análises  
  - `tbl_resultado_covid.csv` – Base consolidada exportada do BigQuery  
  - `README.md` – Este arquivo  
  - `files/`
    - ❌ `brazil_covid19_cities.csv` – Base bruta de casos e óbitos por cidade – [🔗 Buscar no Kaggle](https://www.kaggle.com/datasets/unanimad/corona-virus-brazil)  
    - ❌ `brazil_population_2019.csv` – População estimada por cidade em 2019 – [🔗 Buscar no Kaggle](https://www.kaggle.com/datasets/unanimad/corona-virus-brazil)  
    - `query.txt` – Consulta SQL utilizada no BigQuery
---

## ✍️ Autor

**Jean Santiago**  
Aluno da Pós-graduação em Engenharia de Dados – Instituto Infnet  
Repositório acadêmico para a disciplina de BigQuery – Abril/2025
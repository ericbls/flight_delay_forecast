# USA Flight Delay Forecast

Projeto de Big Data desenvolvido em R para previsão de atrasos em voos nos Estados Unidos, utilizando técnicas de análise exploratória, tratamento de dados e modelagem preditiva em um ambiente distribuído (Databricks + Spark).

## Descrição

O objetivo do projeto é prever a probabilidade de um voo atrasar com base em variáveis históricas e contextuais, como:

* Condições meteorológicas
* Período do ano e horário do voo
* Companhia aérea
* Aeroportos de origem e destino
* Dados operacionais e externos relevantes

A análise utiliza dados massivos (big data) e integra diferentes bibliotecas para manipulação, visualização e modelagem em larga escala.

## Estrutura do Projeto

* **Importação de bibliotecas**

  * `pyspark.sql`, `pyspark.ml` — manipulação e modelagem no Spark
  * `matplotlib`, `seaborn`, `pandas` — visualização e análise exploratória
  * Funções utilitárias (`math`, `window`) para manipulação de dados

* **Etapas Principais**

  1. **Coleta e ingestão de dados** a partir de fontes distribuídas.
  2. **Tratamento e limpeza**: remoção de valores nulos, padronização de formatos e tratamento de outliers.
  3. **Análise exploratória (EDA)**: estatísticas descritivas, visualizações e detecção de padrões.
  4. **Engenharia de atributos**: criação de variáveis derivadas para melhorar o desempenho dos modelos.
  5. **Treinamento e avaliação de modelos preditivos** (ex.: regressão logística, árvore de decisão, random forest).
  6. **Validação e métricas**: acurácia, precisão, recall, AUC-ROC.
  7. **Interpretação e recomendações**.

## Tecnologias Utilizadas

* **Linguagem**: R e PySpark
* **Ambiente**: Databricks Community Edition
* **Bibliotecas**:

  * Manipulação e processamento: `pyspark.sql`, `pyspark.ml`
  * Visualização: `matplotlib`, `seaborn`
  * Análise: `pandas`
* **Big Data**: Apache Spark

## Resultados

* Modelo preditivo capaz de estimar a probabilidade de atraso com base em variáveis meteorológicas e operacionais.
* Insights sobre fatores que mais influenciam atrasos, como condições climáticas adversas e horários de pico.

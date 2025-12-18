# Previsão de Resultados de Partidas da Série A do Campeonato Brasileiro usando Aprendizado de Máquina

Este repositório contém o código-fonte, experimentos e análises desenvolvidos no âmbito do **Projeto Final de Graduação** do curso de **Engenharia de Computação** da **Pontifícia Universidade Católica do Rio de Janeiro (PUC-Rio)**.

O objetivo do trabalho é investigar o uso de técnicas de **Aprendizado de Máquina supervisionado** para a **previsão de resultados de partidas de futebol da Série A do Campeonato Brasileiro**, realizando uma **análise comparativa entre diferentes modelos de classificação**.

---

## Objetivo do Projeto

Desenvolver e avaliar uma *pipeline* de aprendizado de máquina capaz de prever o resultado de partidas de futebol da Série A do Campeonato Brasileiro, considerando:

- **Classificação multiclasse**:
  - Vitória do mandante
  - Empate
  - Vitória do visitante

- **Classificação binária**:
  - Vitória do mandante
  - Não vitória do mandante (empate ou vitória do visitante)

Além da avaliação preditiva, o projeto busca:
- Analisar a **importância dos atributos**
- Investigar o impacto de **engenharia de atributos específica para o futebol brasileiro**
- Comparar métricas adequadas a **dados desbalanceados**

---

## Base de Dados

Os dados utilizados abrangem partidas da **Série A do Campeonato Brasileiro entre 2003 e 2024**, contendo informações como:

- Gols (mandante e visitante)
- Finalizações e finalizações no alvo
- Posse de bola
- Escanteios
- Faltas e cartões
- Métricas pré-jogo 
- Informações contextuais das partidas

As bases foram tratadas individualmente por temporada e utilizadas **sem consolidação permanente em um único arquivo**, respeitando a ordem temporal dos dados.

---

## Engenharia de Atributos

Foram construídos atributos derivados para capturar aspectos relevantes do contexto esportivo brasileiro, incluindo:

- Forma recente das equipes 
- Desempenho como mandante e visitante
- Confrontos diretos 
- Diferenças estatísticas entre mandante e visitante
- Indicadores pré-partida 

Essa etapa é fundamental para representar a natureza dinâmica do futebol e melhorar a capacidade preditiva dos modelos.

---

## Modelos Avaliados

Os seguintes algoritmos de classificação supervisionada foram utilizados:

- Regressão Logística
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Support Vector Machine (SVM)
- Random Forest
- Gradient Boosting
- AdaBoost
- Multi-Layer Perceptron (MLP)
- xgboost

Todos os modelos foram implementados utilizando a biblioteca **scikit-learn**.

---

## Avaliação dos Modelos

As métricas utilizadas incluem:

- Accuracy
- Precision
- Recall
- F1-score (macro e weighted)
- Matrizes de confusão
- Análise por classe (especialmente para empates)



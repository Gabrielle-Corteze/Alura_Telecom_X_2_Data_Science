# 📡 Telecom X - Predição de Churn (Parte 2)

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)

Este repositório contém a segunda etapa do desafio **Telecom X**, focada no desenvolvimento de modelos de Machine Learning para prever a evasão de clientes (Churn).

## 🎯 Objetivo do Projeto
Desenvolver um pipeline de dados capaz de identificar clientes com alta probabilidade de cancelar seus serviços, permitindo que a empresa realize ações preventivas de retenção.

## 🛠️ Tecnologias e Técnicas Utilizadas
- **Linguagem:** Python
- **Pré-processamento:** One-Hot Encoding e Normalização (`StandardScaler`).
- **Tratamento de Desbalanceamento:** SMOTE (Synthetic Minority Over-sampling Technique).
- **Modelos Preditivos:** Regressão Logística e Random Forest.
- **Otimização:** GridSearchCV e Pipelines.
- **Métricas de Avaliação:** Recall, F1-Score e Matriz de Confusão.

## Preparação dos Dados e Modelagem

O processo de preparação foi a base para garantir a alta performance e a confiabilidade dos algoritmos:

   **Classificação de Variáveis:** Identificação criteriosa entre variáveis numéricas (ex: tenure, charges_monthly) e categóricas (ex: contract, internetservice).

  **Codificação (Encoding):**  Aplicação de One-Hot Encoding para converter categorias em formato binário, permitindo que os modelos processem os dados matematicamente.

  **Normalização:** Utilização do StandardScaler para reescalar as variáveis numéricas. Isso impede que variáveis com valores altos (como charges_total) dominem o modelo injustamente frente a variáveis menores.

  **Balanceamento (SMOTE):** Para mitigar o desbalanceamento da base (onde o "Não Churn" era predominante), aplicamos o SMOTE para criar exemplos sintéticos da classe minoritária, resultando em um modelo muito mais sensível à detecção de evasão.

  **Separação de Dados:** Divisão em conjuntos de Treino (80%) e Teste (20%), utilizando o parâmetro stratify para assegurar que a proporção de churn fosse idêntica em ambas as fatias.

## 🔍 Análise Exploratória (EDA) e Insights

A análise dos dados revelou padrões fundamentais que explicam o comportamento dos clientes da Telecom X:

  
  **Principais Descobertas:**

        Impacto do Contrato: Contratos do tipo "mês a mês" são o indicador mais forte de churn. Migrar esses clientes para planos anuais é a estratégia mais eficaz de retenção.

        Ciclo de Vida: O risco de evasão é crítico nos primeiros meses (tenure baixo). Clientes que superam o primeiro ano tendem a se tornar leais.

        Valor Percebido: Mensalidades altas sem a presença de serviços de valor agregado (como onlinesecurity ou techsupport) geram maior rotatividade.

## 🚀 Como Executar o Projeto

Siga os passos abaixo para reproduzir a análise em seu ambiente:
📋 Pré-requisitos

É necessário ter o Python 3.x instalado. Você pode instalar as bibliotecas necessárias com o comando abaixo:
Bash

pip install pandas seaborn matplotlib scikit-learn imbalanced-learn

💻 Instruções de execução

    Clone este repositório para sua máquina local.

    Certifique-se de que o arquivo dados_tratados.csv está na mesma pasta que o notebook.

    Abra o arquivo telecom_x_parte_2.ipynb utilizando o Jupyter Notebook, VS Code ou faça upload para o Google Colab.

    Execute as células em ordem sequencial para processar os dados e visualizar os resultados dos modelos.

---
*Projeto desenvolvido como parte da Formação em Data Science.*

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

## 📈 Principais Insights
Através da análise de importância das variáveis, identificamos que:
1. **Contratos mensais** são o maior gatilho de evasão.
2. O risco de saída é crítico nos **primeiros 6 meses** de adesão.
3. Clientes com **mensalidades elevadas** sem serviços de suporte tendem a cancelar com mais frequência.

## 🚀 Como Executar o Projeto
1. Clone o repositório: `git clone https://github.com/SEU-USUARIO/telecom-x-predicao.git`
2. Instale as dependências: `pip install -r requirements.txt` (se houver)
3. Abra o notebook `telecom_x_parte_2.ipynb` no Google Colab ou Jupyter.

---
*Projeto desenvolvido como parte da Formação em Data Science.*

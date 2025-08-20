# Modelo Preditivo de Evasão de Clientes (Churn) - X-Telecom

-----

### 📝 Sobre o Projeto

Este repositório contém um projeto de ponta a ponta focado na criação de um **modelo preditivo para a evasão de clientes (Churn)** da X-Telecom. O objetivo principal é desenvolver um sistema que possa identificar, com antecedência, os clientes com maior probabilidade de cancelar seus serviços, permitindo que a empresa atue de forma proativa para retê-los.

O projeto passa por todas as etapas do pipeline de Machine Learning, desde a preparação dos dados até a avaliação e interpretação dos modelos.

-----

### 📈 Metodologia e Pipeline de ML

O desenvolvimento do modelo seguiu as seguintes etapas:

  * **Pré-processamento de Dados:** Os dados foram limpos e preparados, com tratamento de valores ausentes, codificação de variáveis categóricas (One-Hot Encoding, binário) e padronização dos dados para otimizar o desempenho dos modelos.
  * **Divisão em Conjuntos de Treino e Teste:** O conjunto de dados foi dividido em 80% para treino e 20% para teste, garantindo uma avaliação justa e imparcial da capacidade de generalização do modelo.
  * **Treinamento de Modelos:** Foram treinados dois modelos de classificação, com abordagens diferentes:
      * **Regressão Logística:** Um modelo linear, simples e rápido, que se beneficia da normalização dos dados.
      * **Árvore de Decisão:** Um modelo não linear que não exige normalização e é excelente para capturar regras de decisão complexas.
  * **Avaliação de Modelos:** As métricas de desempenho foram escolhidas para lidar com o desequilíbrio de classes. A **Matriz de Confusão**, **Precision**, **Recall** e o **F1-Score** foram utilizados para uma avaliação robusta.
  * **Interpretabilidade do Modelo:** A importância das variáveis foi analisada para extrair insights valiosos. Os coeficientes da Regressão Logística e a importância das variáveis da Árvore de Decisão foram investigados para entender quais fatores mais contribuem para a previsão de churn.

-----

### 🎯 Principais Conclusões dos Modelos

A análise dos modelos e de suas variáveis mais relevantes validou a hipótese de que a evasão é previsível e identificou os principais gatilhos:

  * **Tempo de permanência (`tenure`)** foi identificado por ambos os modelos como o principal fator para a retenção de clientes.
  * **Custo mensal (`Charges_Monthly`)** e o **tipo de contrato (`Month-to-month`)** foram consistentemente apontados como fortes indicadores de evasão.
  * A **Regressão Logística** e a **Árvore de Decisão** alcançaram um desempenho promissor, servindo como uma base sólida para a implementação de um sistema de alerta de churn.

-----

### 🛠️ Tecnologias Utilizadas

  * **Python**
  * **Pandas:** Manipulação e análise de dados.
  * **Scikit-learn:** A principal biblioteca para a construção e avaliação dos modelos de Machine Learning.
  * **Matplotlib & Seaborn:** Para a visualização dos dados e das avaliações dos modelos.

-----

### 🚀 Como Executar o Projeto

Para replicar a análise, siga os passos abaixo:

1.  Clone este repositório:
    ```bash
    git clone https://github.com/leocadiok/alura-preditiva-xtelecom.git
    ```
2.  Instale as bibliotecas necessárias:
    ```bash
    pip install pandas numpy scikit-learn matplotlib seaborn
    ```
3.  Abra o notebook `modelo_preditivo.ipynb` (nome a ser confirmado) e execute as células sequencialmente para reproduzir a análise.

-----

### 🧑 Autor

  * @leocadiok

# Sales Forecasting with Machine Learning

Projeto de Machine Learning para previsão de vendas utilizando modelos de regressão.

## Objetivo do projeto

O objetivo deste projeto é construir um modelo capaz de prever o valor de vendas com base em variáveis como preço unitário, quantidade vendida, desconto, loja, categoria e informações temporais.

Este projeto foi desenvolvido com foco em aprendizado prático de Ciência de Dados e construção de portfólio.

## Tipo de problema

Este é um problema de regressão, pois o objetivo é prever um valor numérico: o valor total de vendas.

## Tecnologias utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Scikit-learn
- Joblib
- Jupyter Notebook

## Etapas do projeto

- Definição do problema de negócio
- Criação e carregamento do dataset
- Análise inicial dos dados
- Análise exploratória
- Criação de variáveis temporais
- Tratamento de variáveis categóricas com One-Hot Encoding
- Separação entre treino e teste
- Treinamento de modelos de regressão
- Avaliação com MAE, RMSE e R²
- Comparação entre modelos
- Análise de importância das variáveis
- Salvamento do melhor modelo

## Modelos utilizados

Foram treinados dois modelos:

- Linear Regression
- Random Forest Regressor

## Resultados

| Modelo | MAE | RMSE | R² |
|---|---:|---:|---:|
| Random Forest Regressor | 343.14 | 494.39 | 0.9879 |
| Linear Regression | 1451.34 | 1836.24 | 0.8326 |

O modelo com melhor desempenho foi o Random Forest Regressor, apresentando menor erro e maior capacidade de explicação da variável alvo.

## Principais variáveis

As variáveis mais importantes para a previsão de vendas foram:

- quantidade_vendida
- preco_unitario
- desconto

Esse resultado faz sentido no contexto de negócio, pois o valor final de vendas depende diretamente da quantidade vendida, do preço unitário e do desconto aplicado.

## Estrutura do projeto

```text
sales-forecasting-ml/
│
├── data/
│   └── sales_data.csv
│
├── models/
│   └── random_forest_sales_model.pkl
│
├── notebooks/
│   └── 02_sales_forecasting_ml.ipynb
│
└── README.md
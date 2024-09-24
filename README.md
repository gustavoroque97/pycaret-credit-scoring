# pycaret-credit-scoring

Estamos trabalhando com uma base de dados de crédito, com informações de clientes de um banco utilizando 12 meses de performance. O projeto consistiu dos seguintes passos:

## Descritiva básica univariada e bivariada

## Desenvolvimento do modelo

Desenvolvemos um modelo de regressão logística e avaliamos o seu poder discriminante. 

## Criação de um pipeline

Criamos um pipeline para pré-processamento dos dados numéricos e categóricos contemplando: substituição de valores nulos, One Hot Encoding para variáveis categóricas, Label Encoder para variáveis numéricas e fazendo um Standard Scaler nas variáveis numéricas para colocar as variáveis numa distribuição com média 0 e desvio padrão 1. No pipeline final, fizemos um PCA com 5 componentes e aplicamos a regressão logística. Pela avaliação do modelo, o pré-processamento realizado melhorou o poder discriminante do modelo. 

## Utilização do Pycaret

Através da biblioteca pycaret, criamos um modelo de classificação LightGBM que performou bem em acurácia, apesar de retornar muitos falsos negativos, o que poderia ter sido melhorado com um melhor balanceamento dos dados.

## Deploy do modelo no Streamlit

[streamlit-app_pycaret-2024-09-24-16-09-30.webm](https://github.com/user-attachments/assets/bbc14953-47cb-424d-b025-dae30ed84bc5)

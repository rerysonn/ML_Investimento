# Previsão de Preços de Ações com Machine Learning
Este projeto utiliza algoritmos de Regressão Linear e Random Forest Decision para prever o preço de ações, com base em dados históricos extraídos da API yfinance. O objetivo é fornecer recomendações sobre se o usuário deve comprar, vender ou manter uma ação com base nas previsões de preço. 

## Tecnologias 
 - Python
   - Pandas 
   - NumPy
   - Matplotlib
 - Scikit-Learn
 - Jupyter Notebook
 - yFinance

## Previsão de Preços de Ações Usando Regressão Linear e RandomForestRegressor
Utilizamos a Regressão Linear para prever os preços de ações com base em dados históricos extraídos pela biblioteca yfinance. Este algoritmo é particularmente útil para encontrar relações lineares entre variáveis e foi escolhido devido à sua simplicidade e eficácia na modelagem de tendências de curto prazo no mercado de ações.

### Etapas do algoritmo
**1. Coleta de dados:** Utilizando a API do yFinance para baixar dados historicos das ações, de 2015 a 2024. Entre os dados, esta incluido o fechamento das acoes, que seria o principal alvo do algoritmo.

**2. Preparação de dados:** Calculo de métricas como Média móvel, volatilidade e entre outras. Essas métricas serão usadas como **Features** no treinamento do modelo.

**3. Treinamento do modelo:** Nesta etapa é feita a separação de dados de treino e teste, onde 80% é direcionado a treino e 20% para teste. Também nesta etapa, é feito o calculo de métricas de erro, como o MAE e MSE.
 - OBS: O modelo foi ajusto para prever o fechamento das acoes com base nas features calculadas.
   
**4. Previsões futuras para cada Ação:** Nesta etapa, o modelo foi utilizado para prever a fechamento de acoes futuras para o mês de Agosto. Tendo os mesmos processos que foram executados nas etapas ja citadas.

**5. Comparação de dados:** Para fazer a comparacao de dados, foi utilizado os dados de treinamento reais ate julho e dados previsto pelo modelo, que sao ate o final de agosto. 

## Resultados entre os dois modelos
- Utilizando RegressionLinear:
  
![image](https://github.com/user-attachments/assets/77c738a4-4d2a-421d-8bba-741b329f96ad)
 
- Utilizando o algoritmo de RandomForestRegressor:

![image](https://github.com/user-attachments/assets/a7af8e45-9f7f-482f-903d-1976c8475f7e)

## Contribuintes
- Reryson Farinha
- Diogo Bortolozo






   

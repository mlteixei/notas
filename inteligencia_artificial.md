# Tipos de Algoritmos de Machine Learning

## Aprendizado Supervisionado

### Classificação
- Regressão Logística
- Árvores de Decisão
- Random Forest
- Support Vector Machines (SVM)
- K-Nearest Neighbors (KNN)
- Naive Bayes
- Gradient Boosting Machines (GBM)
- Redes Neurais Convolucionais (CNN)
- Redes Neurais Recorrentes (RNN)

### Regressão
- Regressão Linear
- Regressão de Ridge e Lasso
- Redes Neurais Artificiais
- Gradient Boosting Machines (GBM)
- Máquinas de Vetores de Suporte para Regressão (SVR)
- ElasticNet
- LightGBM
- XGBoost

## Aprendizado Não Supervisionado

### Agrupamento (Clustering)
- K-Means
- Agrupamento Hierárquico
- DBSCAN
- Mean Shift
- Gaussian Mixture Models (GMM)
- OPTICS
- Birch
- Affinity Propagation

### Redução de Dimensionalidade
- Análise de Componentes Principais (PCA)
- t-Distributed Stochastic Neighbor Embedding (t-SNE)
- Autoencoders
- Linear Discriminant Analysis (LDA)
- Independent Component Analysis (ICA)
- Sparse PCA

## Aprendizado por Reforço

### Aprendizado Baseado em Política
- Q-Learning
- SARSA
- Deep Q-Networks (DQN)
- Advantage Actor-Critic (A2C)
- Policy Gradient Methods

### Aprendizado Baseado em Valor
- Algoritmo de Iteração de Valor
- Monte Carlo Control
- Método de Temporal Difference Learning (TD-Learning)
- Deep Deterministic Policy Gradient (DDPG)
- Twin Delayed DDPG (TD3)
- Proximal Policy Optimization (PPO)



# Métricas de Avaliação de Modelos

## Modelos de Classificação

### Acurácia
A acurácia é a proporção de previsões corretas feitas pelo modelo em relação ao total de previsões. A fórmula é:

$$
\text{Acurácia} = \frac{\text{Número de previsões corretas}}{\text{Número total de previsões}}
$$

### Precisão
A precisão é a proporção de previsões positivas que foram corretamente identificadas. A fórmula é:

$$
\text{Precisão} = \frac{\text{Verdadeiros Positivos}}{\text{Verdadeiros Positivos + Falsos Positivos}}
$$

### Recall (Sensibilidade)
O recall é a proporção de valores positivos reais que foram corretamente identificados. A fórmula é:

$$
\text{Recall} = \frac{\text{Verdadeiros Positivos}}{\text{Verdadeiros Positivos + Falsos Negativos}}
$$

### Especificidade
A especificidade é a proporção de verdadeiros negativos em relação ao total de valores reais negativos. É o complemento do recall e indica a habilidade do modelo de evitar falsos alarmes em negativos.

$$
\text{Especificidade} = \frac{\text{Verdadeiros Negativos}}{\text{Verdadeiros Negativos + Falsos Positivos}}
$$

### F1-Score
O F1-Score é a média harmônica entre precisão e recall. A fórmula é:

$$
\text{F1-Score} = 2*\frac{\text{Precisão * Recall}}{\text{Precisão + Recall}}
$$

### Curva ROC e Área sob a Curva (AUC)
A Curva ROC é uma representação gráfica da sensibilidade versus especificidade para um sistema de classificação binário e AUC é a área sob a curva ROC. Quanto maior a AUC, melhor o modelo.

## Modelos de Regressão

### Erro Quadrático Médio (MSE)
O MSE é a média dos quadrados dos erros. Quanto menor o MSE, melhor o modelo. A fórmula é:

$$
\text{MSE} = \frac{1}{n}\sum_{i=1}^{n}(y_i - \hat{y}_i)^2
$$

### Raiz do Erro Quadrático Médio (RMSE)
O RMSE é a raiz quadrada do MSE. É uma medida de desvio padrão dos erros de previsão. A fórmula é:

$$
\text{RMSE} = \sqrt{\frac{1}{n}\sum_{i=1}^{n}(y_i - \hat{y}_i)^2}
$$

### Coeficiente de Determinação (R²)
O R² é uma medida estatística que representa a proporção da variância para uma variável dependente que é explicada por uma variável independente ou variáveis em um modelo de regressão. A fórmula é:

$$
R² = 1 - \frac{\text{Soma dos quadrados dos resíduos}}{\text{Soma total dos quadrados}}
$$

### Erro Absoluto Médio (MAE)
O MAE é a média das diferenças absolutas entre as previsões e os valores reais. Ele fornece uma ideia de quão erradas estão nossas previsões.

$$
\text{MAE} = \frac{1}{n}\sum_{i=1}^{n}|y_i - \hat{y}_i|
$$

### Erro Percentual Absoluto Médio (MAPE)
O MAPE é a média das diferenças percentuais absolutas entre as previsões e os valores reais.

$$
\text{MAPE} = \frac{1}{n}\sum_{i=1}^{n}\left|\frac{y_i - \hat{y}_i}{y_i}\right|
$$

### R² Ajustado
O R² ajustado é uma versão modificada do R² que ajusta o número de preditores no modelo. É útil quando comparamos modelos com diferentes números de preditores.

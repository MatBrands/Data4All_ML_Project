# Estrutura do projeto

## Algoritmo de Machine Learning

Foram escolhidos três modelos em ordem de complexidade e tipo de modelo quanto ao modo de classificação:

- LogisticRegression;
- KNeighborsClassifier;
- RandomForestClassifier.

## Utilização do Random State

- Garantia de que os resultados sejam reproduzíveis.

## Balanceamento de dataset

- Foram realizados testes com o dataset desbalanceado, no qual existia uma proporção de 84 % para "Não" e 16 % para "Sim" quanto a variável "Attrition" que é o alvo do modelo;
- Testes realizados:
	- SMOTE (Synthetic Minority Over-sampling Technique)
	E em conjunto:
	- Random Under-Sampling with Replacement (RUS)
	- Random Over-Sampling with Replacement (ROS)

- Foi escolhida a segunda técnica para balanceamento do dataset, com proporção final de 60 % para "Não" e 40 % para "Sim".
	- Motivo: Maior performance na generalização;

## Divisão do dataset (train / test)

- Foi utilizado train_test_split da biblioteca sklearn para amostragem dos dados; 
- 80% para treino e 20% para teste (como visto em aula).

## Técnicas de tratamento para Categóricas

- Foi utilizado OneHotEncoder() e LabelEncoder() para transformar as variáveis categóricas em numéricas.

## Feature Scaling

- Foram realizados testes para os três modelos citados:
	- LogisticRegression 
	- KNeighborsClassifier 
	- RandomForestClassifier 

## Feature Selection

- Foram removidas ("EmployeeCount", "StandardHours", "Over18");
- Observar as correlações para eliminar as variáveis mais correlacionadas a fim de diminuir o custo do modelo.

### Identificação e eliminação de um variáveis que se comportam como ID.

- "EmployeeNumber" (ID).

## Learning Curve / Underfitting / Overfitting

- Foram abordadas as três questões:

- Aprendizado do modelo;
- Overfitting (modelo aprende demais);
- Underfitting (modelo não aprende o suficiente).

- Foram realizadas curvas de aprendizado em função do número de variáveis empregadas no modelo; 
- Otimizações nos parâmetros para diminuir a possibilidade de Overfitting; 
- Validação Cruzada


## Métricas para avaliação para Classificação/Regressão
### Classificação

Será necessário montar e explicar a matriz de confusão, para assim explicar o foco das métricas:
| Matriz de confusão | --- | Predito | Predito
| --- | --- | --- | ---
| --- | --- | 1 | 0
| Real | 1 | Verdadeiro Positivo (VP) | Falso Negativo (FN)
| Real | 0 | Falso Positivo (FP) | Verdadeiro Negativo (VN)

Erro tipo I (Falso Positivo) - Ocorre quando o modelo prevê que a classe é positiva, mas na verdade é negativa.

Erro tipo II (Falso Negativo) - Ocorre quando o modelo prevê que a classe é negativa, mas na verdade é positiva.

- F1 Score, **Recall (Prioridade)**, Precision Score e Acurácia.

## Pipeline / ColumnTransformer

- Foi utilizado para deixar mais claro a construção do modelo; 
- Automatizar o uso do scaler para diferentes modelos.

## Otimização de Hiperparâmetros

- GridSearchCV (Logistic Regression e KNN;
- RandomizedSearchCV (Random Forest).

## Explicação acerca dos Hiperparâmetros escolhidos

- Logistic Regression:
	- C (Regularização);
	- dual (formulação);
	- fit_intercept (Definir o intercepto da reta);
	- penalty (definir penalidades para o modelo);
	- solver (algorítmo usado na otimização do problema);
	- tol (tolerância ou critério de parada).

- KNeighborsClassifier:
	- n_neighbors (Número de vizinhos utilizados);
	- metric (tipo de distância utilizada nos cálculos);

- RandomForestClassifier:
	- n_estimators (número de estimados utilizados no modelo);
	- min_samples_split (mínimo de amostras para criar um novo nó);
	- min_samples_leaf (número mínimo de amostras requeridas para estar em um ramo);
	- max_depth (regula a profundida da floresta);
	- criterion (critério para medir a qualidade da separação dos ramos);

## Cross Validation

- Foi realizada uma validação cruzada com o objetivo de validar o modelo, para que não haja overfitting.

## Comparativo entre mais de um algoritmo.

Como já discutido, foram comparados três modelos de classificação:

- LogisticRegression.
- KNeighborsClassifier.
- RandomForestClassifier.

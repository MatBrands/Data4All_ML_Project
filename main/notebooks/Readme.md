# Estrutura do projeto

## Algoritmo de Machine Learning (Breve explicação do seu funcionamento)
- LogisticRegression;
- KNeighborsClassifier;
- RandomForestClassifier.

## Utilização do Random State

- Precisamos garantir que os resultados sejam reproduzíveis.

## Balanceamento de dataset

- Realizar testes com o dataset original (desbalanceados), onde existe proporção de 84% pra não e 16% para sim;
- Testar balanceamento através do método de bootstrap, onde tentaremos algo próximo de 60% e 40% (não e sim, respectivamente).

## Divisão do dataset (train / test)

- 80% para treino e 20% para teste (como visto em aula).

## Técnicas de tratamento para Categóricas

- Vamos usar OneHotEncoder() e LabelEncoder() para transformar as variáveis categóricas em numéricas.

## Feature Scaling

- LogisticRegression (Necessário);
- KNeighborsClassifier (Necessário);
- RandomForestClassifier (Não é necessário)

## Feature Selection

- Foram removidas ("EmployeeCount", "StandardHours", "Over18");
- Observar as correlações para eliminar as variáveis mais correlacionadas a fim de diminuir o custo do modelo.

### Identificação e eliminação de um variáveis que se comportam como ID.

- "EmployeeNumber" (ID).

## Learning Curve / Underfitting / Overfitting

- Aprendizado do modelo;
- Overfitting (modelo aprende demais);
- Underfitting (modelo não aprende o suficiente).

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

- F1 Score, **Recall (Prioridade)**, Precision score e Acurácia.

## Pipeline / ColumnTransformer

- Deixar mais claro a construção do modelo; 
- Automatizar o uso do scaler (para diferentes modelos).

## Otimização de Hiperparâmetros

- GridSearchCV;
- RandomizedSearchCV.

## Explicação acerca dos Hiperparâmetros escolhidos

- Através de pesquisas e testes, escolher os melhores hiperparâmetros para cada modelo.

## Cross Validation

- Objetivo de validar o modelo, para que não haja overfitting.

## Comparativo entre mais de um algoritmo.

- LogisticRegression.
- KNeighborsClassifier.
- RandomForestClassifier.
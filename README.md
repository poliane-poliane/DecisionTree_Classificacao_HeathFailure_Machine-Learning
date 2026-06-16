# Árvore de Decisão para Classificação — Heart Failure Prediction

Aplicação de um modelo de Árvore de Decisão a um problema de classificação binária, com o objetivo de prever a tendência de um paciente desenvolver doença cardíaca a partir de indicadores clínicos e laboratoriais. O notebook inclui introdução teórica às principais métricas de avaliação de modelos de classificação, com exemplos didáticos antes da modelagem.

## Dataset

Heart Failure Prediction Dataset — Kaggle (fedesoriano). 918 pacientes, 11 variáveis preditoras, 1 variável-alvo (HeartDisease: 0 = saudável, 1 = doença cardíaca).

**Variáveis preditoras:** Age, Sex, ChestPainType, RestingBP, Cholesterol, FastingBS, RestingECG, MaxHR, ExerciseAngina, Oldpeak, ST_Slope.

## Etapas

- Pré-processamento e inspeção dos dados (shape, describe, checagem de nulos e negativos, dtypes)
- Transformação de variáveis categóricas nominais em ordinais (Label Encoding manual)
- Separação entre variáveis preditoras e variável-alvo
- Divisão treino/teste com `train_test_split` (70/30, random_state=0)
- Treinamento de `DecisionTreeClassifier` (criterion='entropy', max_depth=3)
- Visualização da árvore com `tree.plot_tree`

## Tecnologias

Python, Pandas, NumPy, scikit-learn (DecisionTreeClassifier, train_test_split), Matplotlib.

## Contexto

Projeto de aprendizado pessoal, desenvolvido como prática supervisionada de classificação com dados reais e amplamente conhecidos na comunidade de ciência de dados.

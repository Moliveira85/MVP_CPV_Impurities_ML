# MVP - Predição de Impurezas Totais em Processo Farmacêutico

## Objetivo

Este projeto foi desenvolvido como parte da Sprint de Machine Learning & Analytics da Pós-Graduação em Ciência de Dados e Analytics da PUC-Rio.

O objetivo foi avaliar a viabilidade da utilização de técnicas de Machine Learning para prever níveis de impurezas totais em produtos farmacêuticos a partir de atributos de matéria-prima e processo.

---

## Problema de Negócio

As impurezas representam um importante atributo de qualidade na indústria farmacêutica.

A identificação antecipada de fatores associados ao aumento dos níveis de impurezas pode apoiar estratégias de monitoramento de processo, gestão de risco e Continued Process Verification (CPV).

A pergunta central deste estudo foi:

> É possível utilizar dados de matéria-prima e processo para prever os níveis de impurezas totais observados no produto?

---

## Metodologia

O projeto seguiu as seguintes etapas:

1. Análise exploratória dos dados (EDA);
2. Tratamento e preparação dos dados;
3. Treinamento de modelos de regressão;
4. Comparação de desempenho entre algoritmos;
5. Análise de importância das variáveis;
6. Identificação e remoção de possíveis fontes de vazamento de dados;
7. Revisão dos atributos com base em conhecimento de domínio farmacêutico;
8. Ajuste de hiperparâmetros via Grid Search;
9. Avaliação de overfitting e capacidade de generalização.

---

## Modelos Avaliados

- Regressão Linear
- Random Forest Regressor
- Gradient Boosting Regressor

---

## Principais Resultados

Modelo final:

- Algoritmo: Random Forest Regressor
- Modelo regularizado
- R² Treino: 0,933
- R² Teste: 0,698

Os resultados indicaram capacidade relevante de previsão das impurezas totais utilizando apenas atributos disponíveis no conjunto de dados.

---

## Principais Aprendizados

- Identificação e tratamento de vazamento de dados;
- Seleção de atributos baseada em conhecimento farmacêutico;
- Avaliação de overfitting;
- Aplicação prática de Machine Learning em contexto de CPV.

---

## Trabalhos Futuros

- Classificação de lotes por nível de risco;
- Aplicação em monitoramento baseado em risco;
- Avaliação de impurezas específicas (ex.: nitrosaminas);
- Integração com iniciativas de Farmácia 4.0 e CPV.

---

## Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Scikit-Learn
- Matplotlib
- Seaborn
- Google Colab

---

## Autor

Marcelo Oliveira


Pós-Graduação em Ciência de Dados e Analytics - PUC-Rio

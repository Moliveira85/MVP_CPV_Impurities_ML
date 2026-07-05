# MVP - Inteligência Artificial Aplicada ao Continued Process Verification (CPV)

## Visão Geral

Este projeto apresenta um MVP (Minimum Viable Product) desenvolvido como parte da Pós-Graduação em Ciência de Dados e Analytics.

O objetivo é avaliar a aplicação de técnicas de Machine Learning como ferramenta de suporte às atividades de Continued Process Verification (CPV) na indústria farmacêutica.

Como estudo de caso, foi utilizado o atributo de qualidade **Impurezas Totais (Total Impurities)**, buscando investigar se informações históricas de matérias-primas e processo produtivo podem ser utilizadas para prever o comportamento desse atributo de qualidade.

O foco do trabalho não está exclusivamente na previsão de impurezas, mas na demonstração de uma metodologia de aplicação de Inteligência Artificial para apoio à análise contínua de desempenho de processos farmacêuticos.

---

## Objetivo

Desenvolver e avaliar modelos de Machine Learning capazes de prever um atributo de qualidade farmacêutico a partir de dados históricos de matéria-prima e processo, demonstrando o potencial da Inteligência Artificial como ferramenta de suporte ao Continued Process Verification (CPV).

---

## Dataset

O conjunto de dados utilizado contém atributos relacionados a:

- Matérias-primas;
- Características físico-químicas;
- Variáveis de processo;
- Resultados analíticos;
- Atributos de qualidade.

Os dados foram utilizados exclusivamente para fins educacionais e encontram-se anonimizados, sem identificação de produtos, fabricantes ou informações confidenciais.

---

## Modelos Avaliados

Durante o projeto foram avaliados diferentes algoritmos de regressão:

- Regressão Linear (Baseline);
- Random Forest Regressor;
- Gradient Boosting Regressor.

O Random Forest foi selecionado como modelo principal devido ao melhor equilíbrio entre desempenho preditivo, interpretabilidade e capacidade de generalização.

---

## Principais Etapas do Projeto

### 1. Análise Exploratória de Dados (EDA)

- Distribuição da variável alvo;
- Avaliação dos atributos;
- Correlações;
- Valores ausentes;
- Duplicatas;
- Identificação de padrões relevantes.

### 2. Pré-processamento

- Remoção de colunas de identificação;
- Seleção de atributos numéricos;
- Tratamento de valores ausentes por imputação utilizando mediana;
- Separação entre features e target;
- Divisão treino/teste.

### 3. Modelagem Inicial

- Treinamento dos modelos candidatos;
- Comparação utilizando R², MAE e RMSE;
- Seleção do modelo de melhor desempenho.

### 4. Interpretabilidade

- Análise de Feature Importance;
- Investigação dos atributos mais relevantes;
- Avaliação da plausibilidade farmacêutica das variáveis.

### 5. Identificação de Data Leakage

Uma das contribuições mais importantes do projeto foi a identificação de potenciais fontes de vazamento de dados (*Data Leakage*).

A análise de importância das variáveis revelou que determinados atributos continham informações diretamente relacionadas ao atributo de qualidade previsto.

Após a remoção dessas variáveis, os modelos foram reconstruídos e reavaliados, permitindo uma estimativa mais realista da capacidade de generalização.

### 6. Refinamento e Otimização

- Revisão de atributos baseada em conhecimento de domínio farmacêutico;
- Treinamento de novas versões do modelo;
- Otimização de hiperparâmetros utilizando Grid Search e Cross Validation;
- Avaliação do modelo final.

---

## Métricas Utilizadas

Os modelos foram avaliados utilizando:

- **R² (Coeficiente de Determinação)**
- **MAE (Mean Absolute Error)**
- **RMSE (Root Mean Squared Error)**

Essas métricas permitiram analisar simultaneamente a capacidade explicativa do modelo e o erro associado às previsões.

---

## Principais Aprendizados

Este projeto demonstrou que:

- Técnicas de Machine Learning possuem potencial para apoiar atividades de CPV;
- A qualidade dos atributos utilizados possui impacto significativo no desempenho dos modelos;
- Feature Importance é uma ferramenta importante para interpretação e validação dos resultados;
- Conhecimento de domínio farmacêutico é fundamental para avaliar a aplicabilidade dos modelos;
- A identificação e remoção de Data Leakage pode gerar ganhos mais relevantes que ajustes finos de hiperparâmetros;
- A combinação entre Ciência de Dados e conhecimento de processo é essencial para construção de modelos confiáveis.

---

## Trabalhos Futuros

Possíveis extensões deste estudo incluem:

- Aplicação da metodologia a outros Critical Quality Attributes (CQAs);
- Inclusão de novos conjuntos de dados e produtos;
- Avaliação de técnicas avançadas de interpretabilidade;
- Desenvolvimento de dashboards para monitoramento contínuo;
- Integração com estratégias de monitoramento baseado em risco;
- Exploração de algoritmos avançados de Machine Learning e Explainable AI (XAI).

---

## Aplicação no Contexto Farmacêutico

Embora este estudo tenha utilizado **Impurezas Totais** como variável alvo, a metodologia desenvolvida não está restrita a esse atributo específico.

A abordagem pode ser aplicada a diversos atributos críticos da qualidade (CQAs), tais como:

- Teor;
- Dissolução;
- Umidade;
- Uniformidade de conteúdo;
- Impurezas específicas;
- Outros parâmetros monitorados em programas de Continued Process Verification (CPV).


## Resumo Executivo

Este MVP demonstra a aplicação prática de Machine Learning como ferramenta de suporte ao Continued Process Verification (CPV) na indústria farmacêutica.

Utilizando Impurezas Totais como estudo de caso, foram desenvolvidos modelos preditivos capazes de explorar relações entre atributos de matéria-prima, processo e qualidade do produto.

Mais do que alcançar bons indicadores estatísticos, o projeto evidenciou a importância da interpretação dos resultados, da identificação de vazamento de dados e da utilização de conhecimento de domínio para construção de soluções analíticas confiáveis e aplicáveis em ambientes regulados.

## Autor

Marcelo Oliveira


Pós-Graduação em Ciência de Dados e Analytics - PUC-Rio

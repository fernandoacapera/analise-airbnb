# Análise Exploratória de Dados (EDA) - Airbnb em Nova Iorque

## Visão Geral
Este projeto realiza uma análise exploratória completa do dataset "Airbnb Open Data" de Nova Iorque, disponível no Kaggle. O objetivo é extrair insights sobre o mercado de aluguéis de curta duração na cidade, investigando a distribuição de preços, a popularidade dos imóveis, as características mais comuns e os fatores que podem influenciar as avaliações dos hóspedes.

## Objetivos
O estudo foi guiado pelas seguintes perguntas:

- Como os preços dos imóveis estão distribuídos? Existem muitos outliers?

- Qual a região (neighbourhood group) mais cara e a mais barata de Nova Iorque?

- Qual o tipo de quarto (room type) mais ofertado na cidade?

- Existe alguma correlação entre o preço de um imóvel e a nota de avaliação recebida?

## O Dataset
Fonte: Airbnb Open Data - Kaggle

**Descrição** : O dataset contém 102.599 linhas e 26 colunas, com informações detalhadas sobre os anúncios, incluindo localização, preço, tipo, disponibilidade e avaliações.

**Desafios** : O conjunto de dados original apresentava diversos desafios de limpeza, como dados faltantes, tipos de dados incorretos (preços e taxas como texto) e a necessidade de padronização.

## Ferramentas Utilizadas
Linguagem: Python

## Bibliotecas:

- Pandas para manipulação e limpeza dos dados.

- NumPy para operações numéricas.

- Matplotlib e Seaborn para visualização de dados estática.

## Metodologia
O projeto foi estruturado nas seguintes etapas:

- Coleta e Carregamento dos Dados: Importação do arquivo .csv para um DataFrame do Pandas.

- Limpeza e Pré-Processamento:

- Tradução e padronização dos nomes das colunas.

- Correção dos tipos de dados, principalmente nas colunas price e service fee, removendo caracteres como $ e convertendo para formato numérico.

- Tratamento de valores ausentes (NaN), utilizando estratégias como preenchimento com a mediana para dados numéricos e remoção de linhas/colunas quando apropriado.

- Remoção de outliers de preço para uma análise mais realista da distribuição.

## Análise Exploratória de Dados (EDA):

- Análise estatística descritiva das principais variáveis.

- Investigação da distribuição das variáveis categóricas (região, tipo de quarto).

- Cálculo de correlações entre as variáveis numéricas para identificar possíveis relações.

## Visualização de Dados:

- Criação de gráficos (boxplot e gráficos de barras) para ilustrar os insights encontrados.


## Principais Insights e Visualizações
Aqui estão alguns dos principais resultados encontrados durante a análise:

1. Distribuição de Preços
A maioria dos imóveis tem um preço mais acessível, mas existem alguns imóveis com valores extremamente altos, que foram tratados como outliers. A distribuição dos preços é assimétrica à direita.

<img width="1246" height="701" alt="image" src="https://github.com/user-attachments/assets/3f1854f4-36a2-4868-b66a-ec8a8a6fb37d" />


2. Correlação entre Preço e Avaliação
<img width="515" height="418" alt="image" src="https://github.com/user-attachments/assets/70a120a4-3130-4abf-a71b-cdf4044df83b" />

Isso significa que um preço mais alto não garante, de forma alguma, uma melhor avaliação por parte dos hóspedes. Fatores como custo-benefício e expectativas dos hóspedes provavelmente têm um papel muito mais importante.

## Conclusão
A análise revelou que o mercado de Airbnb em Nova Iorque é fortemente influenciado pela localização, com Manhattan dominando em termos de preços e concentração. O tipo de imóvel mais comum é o "Apartamento/Casa Inteira".

O insight mais valioso, no entanto, é a falta de correlação entre preço e satisfação do cliente, sugerindo que a "qualidade" percebida pelo hóspede é um conceito muito mais complexo do que apenas o valor pago pela diária.

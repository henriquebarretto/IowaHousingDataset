# IowaHousingDataset
# 🏡 Análise e Modelagem Preditiva: Preço de Casas em Ames, Iowa

## ✨ Visão Geral
Este projeto consiste em uma Análise Exploratória de Dados (EDA) aprofundada e no desenvolvimento de um modelo de Machine Learning para prever o preço de venda (`SalePrice`) de casas residenciais na cidade de Ames, Iowa.

O objetivo final é identificar os fatores imobiliários mais influentes (características da propriedade, localização, etc.) e construir um modelo de regressão com alta performance.

## 📊 O Dataset
O estudo utiliza o famoso **Ames Housing Dataset**, que detalha a venda de casas entre 2006 e 2010.
* **Dimensões:** 1460 observações (linhas) e 81 variáveis (colunas).
* **Variável Target (Alvo):** `SalePrice`.

## 🛠️ Tecnologias e Bibliotecas Utilizadas

| Categoria | Biblioteca | Propósito |
| :--- | :--- | :--- |
| **Análise** | `pandas`, `numpy` | Manipulação e processamento de dados. |
| **Visualização** | `matplotlib.pyplot`, `seaborn` | Criação de gráficos estatísticos. |
| **Outras** | `math`, `datetime`, `warnings` | Funções auxiliares e controle de ambiente. |

## 📝 Estrutura e Etapas da Análise

O notebook principal (`Analysis_of_the_Ames,_Iowa_Housing_Dataset.ipynb`) segue a seguinte metodologia de trabalho:

1.  **Configuração Inicial:** Importação de todas as bibliotecas e aplicação de configurações para visualização e reprodutibilidade.
2.  **Carregamento e Inspeção:** Carregamento do dataset e verificação da estrutura, incluindo a inspeção das 81 colunas, tipos de dados (`int64`, `float64`, `object`), e contagem de valores não-nulos.
3.  **Classificação de Variáveis:** Classificação detalhada das 81 variáveis em seus tipos estatísticos para um pré-processamento adequado:
    * **Ordinal** (e.g., `OverallQual`, `KitchenQual`).
    * **Nominal** (e.g., `Neighborhood`, `BldgType`).
    * **Razão** (Variáveis numéricas contínuas e discretas, e.g., `LotArea`, `GrLivArea`, `TotalBsmtSF`).
4.  **Análise dos Dados Brutos:** Geração de estatísticas descritivas das variáveis numéricas principais, como médias, desvios e quartis para `LotArea`, `GrLivArea`, e áreas de porão/garagem.
5.  **Limpeza e Pré-processamento:** Tratamento de valores ausentes (NaN), transformação de variáveis categóricas e tratamento de *outliers*.
6.  **Modelagem:** Aplicação de modelos de regressão (e.g., Linear, Lasso/Ridge, Tree-based) para prever `SalePrice`.
7.  **Avaliação:** Medição da performance dos modelos utilizando métricas como RMSE ou $R^2$.

## 🚀 Como Executar o Projeto

Para reproduzir esta análise em sua máquina local, siga os passos abaixo:

1.  **Clone o repositório**
2.  **Instale as dependências**
3.  **Execute o Notebook:**
    Abra o arquivo `Analysis_of_the_Ames,_Iowa_Housing_Dataset.ipynb` em um ambiente Jupyter (JupyterLab/Colab ou VS Code com extensão Python) e execute as células.

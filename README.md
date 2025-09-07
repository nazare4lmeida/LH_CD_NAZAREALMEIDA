# Desafio de Ciências de Dados | Lighthouse e Indicium: Análise Cinematográfica para a PProductions

## Introdução:

Este projeto foi desenvolvido como parte de um desafio de seleção para a bolsa em Data Science da Indicium, pelo Programa Lighthouse. O objetivo é atuar como um cientista de dados para o estúdio de Hollywood PProductions, utilizando um dataset de filmes do IMDB para guiar a produção de seu próximo sucesso de bilheteria.

A análise abrange desde a exploração inicial dos dados até a aplicação de um modelo preditivo, fornecendo insights detalhados e recomendações.

## Estrutura do Repositório:

O repositório está organizado da seguinte forma:

* `desafio_indicium_imdb.csv`: O dataset original fornecido para a análise.
* `CD_INDICIUM.ipynb`: O relatório principal do projeto. É um Jupyter Notebook contendo toda a análise exploratória de dados (EDA), o processamento de texto, a construção do modelo de machine learning e as conclusões finais, feito através do Google Colabs.
* `desafio_cd_notebook.pkl`: O modelo de regressão linear treinado, salvo no formato .pkl. Este arquivo pode ser carregado e utilizado para fazer novas previsões.
* `requirements.txt`: Arquivo que lista todas as bibliotecas Python e suas versões utilizadas no projeto.

## Como Executar o Projeto

Para reproduzir a análise e o modelo em sua máquina, é só seguir os passos abaixo.

### Pré-requisitos

Certifique-se de ter o Python com a versão mais recente, instalado.

### Passos

1.  Clone este repositório para o seu ambiente local:
    ```bash
    git clone https://github.com/nazare4lmeida/desafio-datascience.git
    ```

2.  Certifique-se de estar no diretório do projeto:
    ```bash
    DESAFIO-DATASCIENCE
    ```

3.  Instale todas as bibliotecas necessárias listadas no `requirements.txt`:
    ```bash
    pip install -r requirements.txt
    ```
4.  Abra o Jupyter Notebook:
    ```bash
    jupyter notebook
    ```

5.  Abra o arquivo `CD_INDICIUM.ipynb` e execute as células para ver a análise completa.

## Principais Conclusões da Análise

* **Fatores de Faturamento:** A análise exploratória demonstrou que o **gênero do filme** é um dos principais fatores relacionados a um alto faturamento, com o gênero Ação liderando a receita total.

* **Influência na Nota IMDB:** A nota da crítica (`Meta_score`) e a popularidade do filme (`No_of_Votes`) mostraram-se fortemente correlacionadas com a nota do público (`IMDB_Rating`), sendo variáveis cruciais para a previsão.

* **Análise de Sinopses:** A nuvem de palavras na coluna `Overview` revelou que temas sobre **"man", "two", "life", "world" e "family", "young"** são recorrentes nas sinopses dos filmes mais aclamados.

* **Modelo Preditivo:** Um modelo de **Regressão Linear** foi treinado com sucesso para prever a nota do IMDB. O modelo atingiu um **Erro Absoluto Médio (MAE)** de **0.20**, indicando uma alta precisão nas previsões.

* **Recomendação de Filme:** Com base na análise, a recomendação para um público desconhecido é um filme com alta nota e alta popularidade. 

* **Nota prevista pro filme modelo:** O modelo previu que a nota do filme 'The Shawshank Redemption' seria de **8.88**.

---

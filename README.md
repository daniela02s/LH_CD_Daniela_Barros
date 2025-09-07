# Indicium | Programa Lighthouse: Desafio de Cientista de Dados
### *Análise de Filmes IMDB para PProductions*

## 1. Visão Geral do Projeto

Este projeto foi desenvolvido como resposta ao desafio de ciência de dados da Lighthouse, simulando uma consultoria para o estúdio de Hollywood **PProductions**. O objetivo principal é analisar uma base de dados cinematográfico para orientar qual tipo de filme deve ser o próximo a ser desenvolvido, extrair insights de negócio e construir um modelo de machine learning capaz de prever a nota de um filme (`IMDB_Rating`), auxiliando o estúdio em suas decisões estratégicas de produção.

A análise completa abrange desde a limpeza e tratamento dos dados, passando por uma análise exploratória (EDA) para identificar padrões, até a engenharia de features, treinamento, otimização e avaliação de modelos preditivos.

## 2. Pré-requisitos

Para executar este projeto, você precisará ter o Python 3.8 (ou superior) instalado, além das bibliotecas listadas no arquivo `requirements.txt`. As principais bibliotecas utilizadas são:

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `nltk`
* `wordcloud`

## 3. Instalação

Para garantir que todas as dependências funcionem corretamente, é recomendável criar um ambiente virtual.

1.  **Clone o repositório:**
    ```bash
    git clone https://[URL-DO-SEU-REPOSITORIO].git
    cd [NOME-DO-SEU-REPOSITORIO]
    ```

2.  **Crie e ative o ambiente virtual:**
    ```bash
    # Para Windows
    python -m venv venv
    .\venv\Scripts\activate

    # Para macOS/Linux
    python3 -m venv venv
    source venv/bin/activate
    ```

3.  **Instale as bibliotecas necessárias:**
    O arquivo `requirements.txt` contém todas as dependências do projeto. Para instalá-las, execute o comando:
    ```bash
    pip install -r requirements.txt
    ```

4.  **Baixe os pacotes do NLTK:**
    Para a análise de texto, é necessário baixar um pacote adicional do NLTK. Abra um interpretador Python (`python` ou `python3` no terminal), e execute os seguintes comandos:
    ```python
    import nltk
    nltk.download('stopwords')
    ```

## 4. Como Executar o Projeto

Toda a análise, desde a importação dos dados até as conclusões finais, está contida no Jupyter Notebook `Lighthouse_CD.ipynb`.

1.  **Inicie o Jupyter:**
    Com o ambiente virtual ativado, execute o seguinte comando no seu terminal:
    ```bash
    jupyter notebook
    ```
    ou, se preferir o Jupyter Lab:
    ```bash
    jupyter lab
    ```

2.  **Execute o Notebook:**
    Na interface do Jupyter que abrirá no seu navegador, clique no arquivo `Lighthouse_CD.ipynb`. Para ver todos os resultados, você pode executar as células sequencialmente, de cima para baixo.

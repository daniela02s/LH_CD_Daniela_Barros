![Indicium Academy Logo](img/indicium_academy_logo.png)
___
# Introdução
Este foi um trabalho/desafio proposto no programa Lighthouse da Indicium.

O programa procura testar conhecimentos dos conceitos estatísticos de modelos preditivos, criatividade na resolução de problemas e aplicação de modelos básicos de machine learning.

O desafio era:

> "Você foi alocado em um time da Indicium contratado por um estúdio de Hollywood chamado PProductions, e agora deve fazer uma análise em cima de um banco de dados cinematográfico para orientar qual tipo de filme deve ser o próximo a ser desenvolvido. Lembre-se que há muito dinheiro envolvido, então a análise deve ser muito detalhada e levar em consideração o máximo de fatores possíveis (a introdução de dados externos é permitida - e encorajada)".
___
Acesse a EDA completa [AQUI](https://github.com/daniela02s/LH_CD_Daniela_Barros/blob/main/Lighthouse_CD.ipynb)
___
# Estrutura do Repositório
O projeto está organizado da seguinte forma:
```
.
├── data/                 # Contém os datasets brutos e processados
├── features/             # Armazena features intermediárias ou processadas
├── Lighthouse_CD.ipynb   # Notebook principal com toda a análise e modelagem
├── modelo_final_imdb.pkl # Modelo de regressão final, serializado e pronto para uso
├── requirements.txt      # Lista de bibliotecas Python necessárias para rodar o projeto
└── README.md             # Documentação do projeto
```
___
# Pré-requisitos

Para executar este projeto, você precisará ter o Python 3.8 (ou superior) instalado, além das bibliotecas listadas no arquivo `requirements.txt`. As principais bibliotecas utilizadas são:

* `pandas`
* `numpy`
* `matplotlib`
* `seaborn`
* `scikit-learn`
* `nltk`
* `wordcloud`
___
# Metodologia
A análise foi dividida em quatro etapas principais:

### 1. Limpeza e Tratamento de Dados:

* Remoção de dados duplicados e tratamento de valores ausentes (NaN).

* Padronização de formatos e conversão de tipos de dados para otimizar a análise.

* Criação de novas features a partir de colunas existentes para enriquecer o dataset.

### 2. Análise Exploratória de Dados (EDA):

* Investigação sobre os gêneros de filmes mais lucrativos e com melhores avaliações.

* Análise da performance de diretores e atores ao longo do tempo.

* Estudo da correlação entre orçamento, receita, e nota do IMDB.

* Visualização de dados para identificar tendências, padrões e insights acionáveis para o estúdio.

### 3. Engenharia de Features:

* Transformação de variáveis categóricas em formato numérico para uso no modelo.

* Seleção das features mais relevantes com base na análise exploratória para prever a nota do IMDB.

### 4. Modelagem Preditiva:

* Treinamento de um modelo de regressão para prever a variável alvo imdb_score.

* Otimização de hiperparâmetros para maximizar a performance do modelo.

* Avaliação do modelo final utilizando métricas como o Erro Quadrático Médio (RMSE).

* O modelo final foi salvo no arquivo modelo_final_imdb.pkl.
___

# Instalação

Para garantir que todas as dependências funcionem corretamente, é recomendável criar um ambiente virtual.

1.  **Clone o repositório:**
    ```bash
    git clone https://LH_CD_Daniela_Barros.git
    cd LH_CD_Daniela_Barros
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

# Como Executar o Projeto

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

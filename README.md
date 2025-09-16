# Desafio Cientista de Dados - PProductions

Este projeto tem como objetivo a análise de dados de filmes para auxiliar o estúdio PProductions na seleção de produções com maior potencial de sucesso, além de prever a nota IMDb de novos filmes com base em características históricas como duração, numero de votos, nota da crítica e bilheteria.

## Estrutura do Projeto

```bash
/desafio-filmes/
    notebooks/
        algoritmo_eda_modelagem.ipynb
    reports/
        relatorio_EDA_filmes.html
        metricas_modelo.txt
    models/
        imdb_pipeline.pkl
    data/
        classificacao_filmes_imdb.csv
    requirements.txt
    README.md
```

## Como Executar o Projeto

1. Efetuar a clonagem de repositório:

```bash
git clone <URL_REPO>
cd desafio-filmes
```

2. Criar e ativar um ambiente virtual (opcional, mas recomendado):

```bash
python -m venv venv
source venv/bin/activate # Linux/Mac
venv\Scripts\activate # Windows
```

3. Instalar as dependências necessárias:

```bash
pip install -r requiments.txt
```

4. Abrir e executar o notebook:

```bash
jupyter notebook notebooks/algorimo_eda_modelagem.ipynb
```

5. Saída Principal:

O modelo final será salvo no seguinte caminho de arquivo:

```bash
models/IMDb_pipeline.pkl
```

## Resultados

- MAE: 0.1623
- RMSE: 0.2048
- R²: 0.3609

Modelo elaborado em Random Forest Regressor por meio da aplicação de: 

- Pré-processamento automático com ColumnTransformer e Pipeline
- Busca de hiperparâmetros com RandomizedSearchCV
- Validação Cruzada com K-Fold

## Ferramentas Utilizadas

- Python (3.10+)
- Pandas, Numpy (Manipulação e transformação dos dados)
- Scikit-learn (modelagem, métricas, pré-processamento)
- ydata-profiling (EDA Automatizado)
- Matplotlib, Seaborn (Visualização Gráfica)
- Joblib (salvar e carregar modelos treinados)

## Próximas etapas e Aprimoramentos Futuros

- Aplicar técnicas de seleção de variáveis para melhorar interpretatbilidade
- Aprimorar tratamento de valores nulos e variáveis categóricas para futuros datasets
- Experimentar outros algoritmos de machine learning como Gradient Boosting ou XGBoost

## Autoria
- Nome: Marcus Vinícius Gonçalves de Souza Couto
- Contato: 
# Desafio Cientista de Dados - PProductions

## Introdução

Este projeto foi desenvolvido como parte do desafio de Cientista de Dados da Indicium. O objetivo é realizar uma análise de dados cinematográficos para orientar PProductions sobre o tipo de filme que deve ser desenvolvido a seguir.

## Estrutura do Projeto

- `EDA.pdf/`: Contém o PDF com a análise exploratória de dados (EDA).
- `EDA.ipynb/`: Contém o Jupyter Notebook, com a análise exploratória de dados (EDA).
- `modelo_preditivo_imdb.pkl/`: Contém o modelo salvo em formato `.pkl`
- `modelo_preditivo_imdb.ipynb/`: Contém o Jupyter Notebook para a ciração do modelo preditivo.
- `respostas.pdf/`: Contém a respostas as perguntas dos passos 2, 3 e 4 do desafio em formato PDF.
- `Previsão.ipynb/`: Contém o Jupyter Notebook usado para testar o modelo preditivo com filmes do dataset.
- `respostas.ipynb/`: Contém a respostas as perguntas dos passos 2, 3 e 4 em um Jupyter Notebook.
- `requirements.txt`: Lista de pacotes Python necessários.
- `README.md`: Instruções sobre como instalar e executar o projeto.
- `desafio_indicium_imdb.csv`: Dataset fornecido pela Indicium e usado no projeto.

## Instalação

1. **Clone o repositório:**

   ```bash
   https://github.com/GustavoSSSSilva/LH_CD_GustavoSilva.git
   cd desafio-cientista-dados

2. **Crie um ambiente virtual:**

   ```bash
   python -m venv venv
   source venv/bin/activate  # Para Windows: venv\Scripts\activate

3. **Instale os pacotes necessários:**

   ```bash
   pip install -r requirements.txt

## Execução
- `Análise Exploratória de Dados (EDA):/`: Abra o pdf EDA.pdf ou o Jupyter Notebook EDA.ipynb para visualizar a análise exploratória dos dados.
- `Modelagem Preditiva:/`: O notebook Modelo_preditivo.ipynb contém o modelo de previsão de notas IMDb.
- `respostas:/`: As respostas das perguntas estão disponíveis em respostas.pdf e em respostas.ipynb.
- `Modelo Salvo:/`: O modelo preditivo treinado está salvo em modelo_preditivo_imdb.pkl. Você pode carregá-lo em Python para fazer previsões.
- `Testar Modelo:/`: O modelo preditivo pode ser usado no arquivo Previsão.ipynb para prever a nota filmes do dataset.
  
  ## Carregando o Modelo

Para carregar o modelo salvo e fazer previsões, utilize o seguinte código em Python:

```python
import pickle

with open('models/imdb_rating_model.pkl', 'rb') as file:
    model = pickle.load(file)

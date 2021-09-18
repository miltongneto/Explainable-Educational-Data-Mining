# Explainable-Educational-Data-Mining
Mineração de Dados Educacionais (Educational Data Mining) com Explainable AI

O código principal do projeto está na pasta *notebooks*, onde os arquivos estão numerados de acordo com a lógica de execução e seguindo o processos comuns em Ciência de Dados.
Na pasta *notebooks*:
- Os arquivos os arquivos *eda* (de *Exploratory Data Analysis*) são os primeiros a serem executados (ou apenas lidos). Nesses arquivos é realizado uma análise e manipulação dos dados. Resultando uma base de dados transformada e salva em *data/processed*. Este resultado conta com agregação e mudança de grão (ou nível) dos dados brutos, em geral passando para o grão escola, além da limpeza, tratamento, criação de atributos, etc.
- O primeiro arquivo que deve ser executado é o 00-eda-saresp.ipynb. Ele deve ser o primeiro pois algumas arquivos de *EDA* utilizam ele.
- A ordem dos arquivos *01-eda-\** não tem interfere no resultado ou entendimento.
- Em *02-feature_engineering.ipynb*, é realizado a preparação dos dados para etapa de Machine Learning. Exercendo o refinamento do tratamento feito na etapa anterior, juntando as diversas bases e criando novas features (atributos).
- Na etapa de modelagem, em *03-machine_learning.ipynb*, é construído um classificador para predizer se uma escola terá desempenho bom ou ruim no SARESP (Sistema de Avaliação de Rendimento Escolar do Estado de São Paulo). O intuito é alcançar uma taxa elevada de assertividade e mapear bem as características da escola, que incluem fatores externos e aspectos da gestão escolar.
- Depois de construir o modelo e alcançar um bom desempenho, é feita a interpretabilidade do modelo em *04-explainable-ai.ipynb*. Nesta fase, são aplicadas as técnicas SHAP e Counterfactual de Explainable AI para inspecionar o modelo.

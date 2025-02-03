# Modelo de Regressão Linear para Previsão de Vendas - 
## Análise Detalhada
Este repositório contém um script Python que implementa um modelo de regressão linear para prever vendas com base em gastos com publicidade em diferentes mídias (YouTube, Facebook e jornal). O código utiliza as bibliotecas Pandas, Seaborn e Scikit-learn, e inclui uma análise exploratória detalhada dos dados, limpeza, pré-processamento e avaliação do modelo.

## Arquivos
MKT.csv: Conjunto de dados contendo informações sobre gastos com publicidade e vendas.
regressao_linear.ipynb: Notebook Jupyter com o código Python comentado.
README.md: Este arquivo.

## Dependências
Para executar o código, você precisa ter as seguintes bibliotecas instaladas:

pandas
seaborn
numpy
plotly
cufflinks
chart-studio
scikit-learn
matplotlib

Você pode instalá-las usando o pip:

pip install pandas seaborn numpy plotly cufflinks chart-studio scikit-learn matplotlib

## Como usar
Clone este repositório:

git clone https://[endereço-do-repositório].git
Abra o notebook Jupyter regressao_linear.ipynb em seu ambiente local.

Certifique-se de que o arquivo MKT.csv esteja no mesmo diretório que o notebook.

Execute as células do notebook para realizar a análise e treinar o modelo.

## Descrição do código
O código realiza as seguintes etapas:

### 1.Importação das bibliotecas:

Importa as bibliotecas necessárias para manipulação de dados, visualização e modelagem.

### 2.Carregamento e exploração inicial dos dados:
Carrega o dataset MKT.csv usando Pandas, definindo a vírgula como separador.
Exibe as primeiras linhas do dataset usando head().
Exibe informações sobre os tipos de dados e número de entradas usando info().
Gera estatísticas descritivas das variáveis numéricas usando describe().

### 3.Limpeza e pré-processamento dos dados:
Verifica a presença de valores nulos em cada coluna usando isnull().sum().
Remove linhas com valores nulos, se existirem, usando dropna().
Verifica a presença de duplicatas no dataset usando duplicated().sum().
Calcula o IQR (Intervalo Interquartil) para detecção de outliers.
Identifica valores outliers nas colunas usando o critério de 1.5 vezes o IQR.
Remove outliers do dataset usando indexação booleana.
Remove duplicatas do dataset usando drop_duplicates().
Verifica o estado do dataset após a limpeza usando info().

### 4.Visualização e análise exploratória de dados (EDA):
Instala as bibliotecas de visualização plotly, cufflinks e chart-studio.
Importa as bibliotecas de visualização e outras necessárias.
Cria um boxplot interativo para identificar outliers nas variáveis usando plotly.express.
Exibe as colunas do dataset usando columns.
Cria pairplots para visualizar a relação entre as variáveis usando seaborn.pairplot().
Cria pairplots especificamente entre os investimentos e as vendas.
Calcula a matriz de correlação entre as variáveis usando corr().
Cria um mapa de calor (heatmap) para visualizar as correlações usando seaborn.heatmap().
Cria histogramas para visualizar a distribuição das variáveis usando seaborn.histplot().

### 5.Preparação dos dados para o modelo:
Separa as variáveis independentes (X) e a variável dependente (Y).
Divide os dados em conjuntos de treino e teste usando train_test_split().

### 6.Treinamento e avaliação do modelo de regressão linear:
Importa e cria um modelo de regressão linear usando LinearRegression().
Treina o modelo com os dados de treino usando fit().
Realiza predições com o conjunto de teste usando predict().
Calcula o coeficiente de determinação (R²) para avaliar o modelo usando r2_score().
Plota as predições versus os valores reais usando matplotlib.pyplot.

### 7.Estatísticas descritivas:
Exibe as estatísticas descritivas do dataset mais uma vez para revisão usando describe().

## Resultados
O código gera um modelo de regressão linear que pode ser usado para prever vendas com base nos gastos com publicidade. O R² é utilizado para avaliar a qualidade do modelo. O gráfico de predições versus valores reais permite visualizar o desempenho do modelo.

## Observações
O código foi desenvolvido em Python 3.
O arquivo MKT.csv deve conter as colunas 'youtube', 'facebook', 'newspaper' e 'sales'.
O modelo de regressão linear é uma abordagem simples e pode não ser o mais adequado para todos os casos. Modelos mais complexos podem ser explorados dependendo da natureza dos dados.

## Contato
Se tiver alguma dúvida ou sugestão, entre em contato:

[Charles William]
[c_wasouza@outlook.com]

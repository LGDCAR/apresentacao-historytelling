Markdown

Classificando a Qualidade de Vinhos com Machine Learning
Este repositório contém o projeto do **Tech Challenge**, desenvolvido como atividade obrigatória para a conclusão da fase corrente. O objetivo principal é utilizar a inteligência artificial para prever se um vinho possui alta qualidade com base em suas características físico-químicas.

Objetivo do Desafio

O mercado de vinhos depende muito da avaliação humana (sensorial), que pode ser demorada e subjetiva. Este projeto cria um modelo preditivo baseado no    Wine QT para automatizar esse processo, transformando as notas dos especialistas em uma classificação binária:
Alta Qualidade: Nota igual ou maior que 7.
Baixa/Média Qualidade: Nota menor que 7.

Estrutura do Repositório

O projeto está organizado da seguinte forma:
Classificação da Qualidade do Vinho
├── data/           # Base de dados original (wineQT.csv)
├── notebooks/      # Colab Notebook com a análise (EDA) e treinamento
├── src/            # Scripts auxiliares de processamento e modelagem
├── resultados/     Gráficos gerados (Matriz de confusão, importância de variáveis)
├── requirements.txt# Bibliotecas necessárias (pandas, scikit-learn, seaborn, etc.)
└── README.md       # Descrição e instruções do projeto (Este arquivo)

Principais Descobertas (Insights de Negócio)

Após a Análise Exploratória de Dados (EDA), descobrimos que:
1. Teor Alcoólico (Alcohol): É o fator de maior impacto positivo. Vinhos mais bem avaliados tendem a possuir um teor alcoólico ligeiramente maior.
2. Acidez Volátil (Volatile Acidity): Possui forte impacto negativo. Quanto maior a presença de acidez volátil (que remete ao gosto de vinagre), menor é a nota atribuída pelos especialistas.

Modelagem e Resultados

Testamos dois modelos de Machine Learning utilizando dados padronizados (`StandardScaler`):
1. Regressão Logística
2. Random Forest (Floresta Aleatória)
O Modelo Vencedor: O algoritmo Random Forest apresentou o melhor desempenho geral (Acurácia), mostrando-se altamente robusto para identificar os padrões químicos que definem um vinho premium.

Como Executar o Projeto

1.	Copie este repositório:
 https://github.com/LGDCAR/apresentacao-historytelling/blob/main/postechchallenge_fase2_.ipynb
2. Instale as bibliotecas necessárias:
 pandas , numpy , matplotlib.pyplot , seaborn 
sklearn.model_selection import train_test_split
preprocessing import StandardScaler
 sklearn.linear_model import LogisticRegression
 sklearn.ensemble import RandomForestClassifiersklearn.metrics import classification_report, accuracy_score, confusion_matrix, precision_score, recall_score pip install -r requirements.txt
Baixo o df = wineQT.csv
3. Abra e execute o notebook na pasta `notebooks/` postechchallenge-fase2 .ipynb

 Nome : Luis Gustavo de Carvalho RM 370823
________________________________________

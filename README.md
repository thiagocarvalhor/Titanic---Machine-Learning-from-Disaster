# Titanic - Machine Learning from Disaster
Bem-vindo à lendária competição Titanic ML, uma excelente oportunidade para entrar no mundo das competições de aprendizado de máquina e se familiarizar com a plataforma Kaggle.

Link para a competição: Titanic - Machine Learning from Disaster

Dicionário de Dados:
Variáveis e Definições
Sobrevivência: Indica se o passageiro sobreviveu ou não. (0 = Não, 1 = Sim)
Classe: Classe do bilhete do passageiro. (1 = 1ª classe, 2 = 2ª classe, 3 = 3ª classe)
Sexo: Gênero do passageiro.
Idade: Idade do passageiro em anos.
SibSp: Número de irmãos/cônjuges a bordo do Titanic.
Parch: Número de pais/filhos a bordo do Titanic.
Bilhete: Número do bilhete do passageiro.
Tarifa: Tarifa paga pelo passageiro.
Cabine: Número da cabine do passageiro.
Embarque: Porto de embarque do passageiro. (C = Cherbourg, Q = Queenstown, S = Southampton)
Bibliotecas Utilizadas:
python
Copy code
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
from sklearn.model_selection import train_test_split
from sklearn.linear_model import LinearRegression
from sklearn.tree import DecisionTreeClassifier
from sklearn.metrics import accuracy_score
from sklearn.neighbors import KNeighborsClassifier
from sklearn.linear_model import LogisticRegression
from sklearn.ensemble import RandomForestClassifier
from sklearn.svm import SVC
import xgboost as xgb
from sklearn.metrics import confusion_matrix
Uso do Código:
Importando os Dados:
python
Copy code
train = pd.read_csv('train.csv')
test = pd.read_csv('test.csv')
Pré-processamento dos Dados:
Preenchimento dos valores faltantes na coluna 'Age' com a média das idades.
Preenchimento do valor faltante na coluna 'Fare' do conjunto de teste com a média das tarifas.
Modelagem e Avaliação:
Divisão dos dados em conjuntos de treinamento e teste.
Treinamento de vários modelos de classificação, como Árvore de Decisão, KNeighborsClassifier, Regressão Logística, Random Forest, SVM e XGBoost.
Avaliação do desempenho dos modelos usando métricas como acurácia e matriz de confusão.
Conclusões:
Após explorar e pré-processar os dados do conjunto de dados do Titanic, foram construídos e avaliados vários modelos de aprendizado de máquina para prever a sobrevivência dos passageiros. Dentre os modelos testados, a regressão logística demonstrou ser a mais promissora, apresentando uma acurácia de aproximadamente 66,75% nos dados de teste. Embora haja espaço para melhorias e refinamentos adicionais, este resultado inicial fornece uma base sólida para futuras iterações e otimizações do modelo.

## Sobre o Autor:
Saiba mais sobre o autor deste projeto:
- [Thiago Ribeiro](https://www.linkedin.com/in/thiago-carvalho-ribeiro-a7ba64208/)

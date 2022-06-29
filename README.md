# Repository Machine Learning
![GitHub](https://img.shields.io/github/license/IgorDamascenoM/Repository2RP?style=social)

# Sobre o Projeto
Repositório criado para apresentação da análise de dados e machine learnig para predição de diabetes

## Importação das bibliotecas que serão utilizadas 
##### Nesse projeto utilizei NumPy, Pandas, MatplotLib, Joblib, SeaBorn e ScikitLearn

```Python 

import numpy as np
import pandas as pd
import matplotlib as mat
import matplotlib.pyplot as plt
import joblib 
import seaborn as sns
import sklearn as sk
from sklearn import metrics
from sklearn.linear_model import LogisticRegression # Modelo de regressão linear
from sklearn.preprocessing import MinMaxScaler # Para transformar os dados
from sklearn.model_selection import train_test_split # Para dividir o banco de dados
from sklearn.neighbors import KNeighborsClassifier # Modelo KNN
from sklearn.tree import DecisionTreeClassifier #Decision Tree Model
from sklearn.neural_network import MLPClassifier #MLP Model


from sklearn.metrics import classification_report, confusion_matrix, accuracy_score 
%matplotlib inline

```

## Importando o arquivo e verificando os dados

```Python
df_diabetes = pd.read_csv('dados_DM.csv', delimiter =',')
```
```Python
df_diabetes.head(5)
```
![9B4132CF-E6C5-4BC8-A915-562B0023D8E2_4_5005_c](https://user-images.githubusercontent.com/96548834/176537788-4790bb2c-95ee-4076-9f30-fac909203b2a.jpeg)

```Python
df_diabetes.tail(5)
```
![A5D5B0FD-EBC6-46D1-AAE6-1FF8162EB5CF_4_5005_c](https://user-images.githubusercontent.com/96548834/176538944-456b4f79-c006-4cdb-bcb3-f550b19125ac.jpeg)

```Python
df_diabetes.columns
```
Index(['Pregnancies', 'Glicose', 'PS', 'EP', 'Insulina', 'IMC',
       'PedigreeDiabetes', 'Idade', 'Diabete'],
      dtype='object')
# Arquivos usados para realizar a atividade
[SQL_Knowledge.zip](https://github.com/IgorDamascenoM/Repository-SQL/SQL_Knowledge.zip)

# Autor
Igor Damasceno Mota

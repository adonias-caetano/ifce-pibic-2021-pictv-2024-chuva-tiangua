 # Avaliação de Desempenho de Classificadores a Partir de Dados Relacionados a Precipitação Pluviométrica Coletados por Estação Meteorológica Automática.

<p align="center">
Este repositório fornece scripts relacionados à previsão de precipitações do município de Tianguá (CE) utilizando algoritmos de Machine Learning (ML) e método de explicabilidade Local Interpretable Model-Agnostic Explanations (LIME).
  
O projeto de pesquisa é fruto de orientação e coordenação do Prof. Me. Rhyan Ximenes de Brito, docente do Instituto Federal do Ceará (IFCE) Campus Tianguá, juntamente com os seguintes pesquisadores e autores do curso de Bacharelado de Ciência da Computação (BCC):

* Ananias C. de Oliveira (concludente do BCC, bolsista PIBIC/IFCE 2020-2021)
* Maria Auxiliadora de Oliveira Chaves (discente do BCC, bolsista PICTV/IFCE 2024-2025)
* Roney Nogueira de Sousa (concludente do BCC, discente Programa de Pós-Graduação em Ciência da Computação (PPGCC) do IFCE)
* Adonias Caetano de Oliveira (coorientador do porjeto, docente do IFCE, discente do Programa de Pós-Graduação em Biotecnologia (PPGBiotec) da Universidade Federal do Delta do Parnaíba (UFDPar)) 
* Paulo César de Almeida Júnior (docente do IFCE, coordenador PICTV)

</p>


<div align="justify">

 ## 📋 Requisitos

* Google Colab
* python pandas
* python numpy
* python plotly
* python seaborn as sns
* python matplotlib
* python tqdm
* python imblearn.under_sampling RandomUnderSampler
* python scipy
* python sklearn.manifold TSNE
* python sklearn.ensemble RandomForestClassifier
* python sklearn.svm SVC
* python sklearn.neighbors KNeighborsClassifier
* python sklearn.neural_network MLPClassifier
* python sklearn.naive_bayes GaussianNB
* python sklearn.linear_model LogisticRegression
* python sklearn.ensemble ExtraTreesClassifier
* python sklearn.model_selection GridSearchCV
* python sklearn.pipeline Pipeline
* python sklearn.model_selection train_test_split
* python sklearn.metrics classification_report
* python sklearn.ensemble VotingClassifier
* python lime lime_tabular
* python sklearn.metrics confusion_matrix, accuracy_score, precision_score, recall_score, f1_score
  
## 📖  Conjunto de Dados

https://zenodo.org/records/14914786

O <a href="https://zenodo.org/records/14914786"><strong>conjunto de dados</strong></a>, denominado Conjunto de Dados Tiangua (A368) de Precipitações, foi coletado por meio de uma estação meteorológica automática localizada em Tianguá, um município do Estado do Ceará. Ela pode ser encontrada no banco de dados do Instituto Nacional de Meteorologia (INMET) do Brasil. Os dados foram coletados entre 15/03/2018 e 11/05/2021, gerando assim um total de 27655 registros.

O conjunto de dados é composto por 19 atributos, as quais representam as grandezas relativas à temperatura do ar, umidade relativa do ar, temperatura do ponto de orvalho, pressão atmosférica do ar, velocidade do vento, direção do vento, intensidade da rajada do vento e radiação solar, em que algumas dessas categorias variam entre valor instantâneo, mínimo e máximo.

## 🛠 Ajuste fino de modelos clássicos de ML

Este estudo exploratório realizou uma análise comparativa de desempenho dos algoritmos Logistic Regression (LR), Naive Bayes (NB), Extra Tree (ET), Extreme Learning Machine (ELM), k-nearest neighbors (k-NN), Multilayer Perceptron (MLP), Random Forest (RF), Support Vector Machines (SVM) e um modelo ensemble na identificação de precipitações. Para avaliação de desempenho foram adotadas as métricas de acurácia, precisão, sensibilidade (ou recall) e medida-F1 (F1-macro). 

Os experimentos computacionais foram implementados utilizando a linguagem de programação Python mediante Google Colaboratory. Os algoritmos foram implementados usando a biblioteca Scikit-learn realizando ajuste fino dos algoritmos pelo método GridSearch. O conjunto de dados foi dividido em 80% para treinamento e validação dos algoritmos mediante a validação cruzada 10-fold e 20% para teste dos modelos. 

Ademais, a decisão sobre o melhor modelo de ML entre os modelos avaliados neste estudo pode ser questionada, pois o desempenho dos modelos de ML pode variar conforme o conjunto de dados. Assim, como contribuição deste trabalho, foi abordado a explicabilidade do melhor modelo utilizando o método Local Interpretable Model-Agnostic Explanations (LIME) para determinar o modelo mais adequado para previsão. Essa análise é útil para determinar os atributos do conjunto de dados que mais influenciam na classificação, ou seja, mostrar caminhos para melhorar a classificação em trabalhos futuros que podem, por exemplo, aplicar seleção de atributos.

## 🤖 Acesso ao artigo submetido

Os resultados deste estudo foram compilados em artigo científico submetido e sob revisão na <a href="https://seer.ufrgs.br/reic"> <strong>Revista Eletrônica de Iniciação Científica em Computação</strong></a>

### [Paper Link]

## 👏 Contribuindo

Se houver um bug ou outra melhoria que você gostaria de relatar ou solicitar, nós o encorajamos a contribuir.

Por favor, sinta-se à vontade para entrar em contato conosco para quaisquer perguntas: [![Gmail Badge](https://img.shields.io/badge/-adonias.oliveira@ifce.edu.br-c14438?style=flat-square&logo=Gmail&logoColor=white&link=mailto:adonias.oliveira@ifce.edu.br)](mailto:adonias.oliveira@ifce.edu.br )


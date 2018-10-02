# udacity_project02

Visão geral do projeto
- Neste projeto, você vai analisar um conjunto de dados e, em seguida, comunicar suas conclusões sobre o assunto. Você vai usar as bibliotecas NumPy, Pandas e Matplotlib para facilitar sua análise.

O que é necessário instalar?
- Você precisará instalar o Python, além das seguintes bibliotecas:

* pandas
* numpy
* matplotlib
* csv
Recomendamos a instalação do Anaconda, que vem com todos os pacotes necessários, bem como o notebook iPython.

Por que este projeto?
- Este projeto irá apresentar você ao processo de análise de dados que será usado em todo o resto do programa Nanodegree. Nele, você vai passar por todo o processo para compreender como todas as peças se encaixam. Mais adiante, os projetos do Nanodegree focarão nas partes individuais do processo de análise de dados. Neste projeto, você também vai adquirir experiência usando as bibliotecas Numpy, Pandas e Matplotlib, que facilitam muito a escrita de códigos.

O que vou aprender?
Após a conclusão do projeto, você irá:
- Saber todos os passos envolvidos em um processo de análise de dados típico
- Sentir-se confortável para fazer perguntas que podem ser respondidas por um conjunto de dados e, em seguida, respondê-las
- Saber como investigar problemas em um conjunto de dados e confrontrar os dados em um formato que você possa usar
- Adquirir prática em comunicar os resultados de sua análise
- Ser capaz de usar as operações vetorizadas no NumPy e Pandas para acelerar seu código de análise de dados
- Ter familiaridade com objetos, séries e o banco de dados Pandas, que permitem acessar seus dados de forma mais conveniente
- Saber usar o Matplotlib para produzir gráficos mostrando suas descobertas

Por que isso é importante para minha carreira?
- Com este projeto, você conseguirá diversas habilidades em análise de dados e, ainda, poderá mostrar a potenciais empregadores que sabe produzir todo o processo de análise de dados



- INTRODUÇÃO
Esse relatório faz parte do projeto de conclusão de Fundamentos de Data Science I da Udacity. Esse projeto tem o objetivo de analisar um conjunto de dados demográficos e outras informações relativas de 891 das 2.224 pessoas a bordo do Titanic.

O RMS Titanic foi um navio de passageiros britânico operado pela White Star Line e construído pelos estaleiros da Harland and Wolff em Belfast. Foi a segunda embarcação da Classe Olympic de transatlânticos depois do RMS Olympic e seguido pelo HMHS Britannic. Projetado pelos engenheiros navais Alexander Carlisle e Thomas Andrews, sua construção começou em março de 1909 e ele foi lançado ao mar em maio de 1911. O Titanic foi pensado para ser o navio mais luxuoso e mais seguro de sua época, gerando lendas que era supostamente "inafundável".

A embarcação partiu em sua viagem inaugural de Southampton para Nova Iorque em 10 de abril de 1912, no caminho passando em Cherbourg-Octeville na França e por Queenstown na Irlanda. Ele colidiu com um iceberg às 23h40min do dia 14 de abril e afundou na madrugada do dia seguinte com mais de 1 500 pessoas a bordo, sendo um dos maiores desastres marítimos em tempos de paz de toda a história. Seu naufrágio destacou vários pontos fracos de seu projeto, deficiências nos procedimentos de evacuação de emergência e falhas nas regulamentações marítimas da época. Comissões de inquérito foram instauradas nos Estados Unidos e no Reino Unido, levando a mudanças nas leis internacionais de navegação que permanecem em vigor mais de um século depois.

source: https://pt.wikipedia.org/wiki/RMS_Titanic



Origem da base:
O dataset é oriundo do site do Kaggle, a maior comunidade de Data Scientists e Machine Learners.

Link: https://www.kaggle.com/c/titanic/data



Descrição das variáveis do dataset:
Para nos auxiliar na interpretação do dataset, é possível verificar a legenda dos dados:

- Survived: Outcome of survival (0 = No; 1 = Yes)
- Pclass: Socio-economic class (1 = Upper class; 2 = Middle class; 3 = Lower class)
- Name: Name of passenger
- Sex: Sex of the passenger
- Age: Age of the passenger (Some entries contain NaN)
- SibSp: Number of siblings and spouses of the passenger aboard
- Parch: Number of parents and children of the passenger aboard
- Ticket: Ticket number of the passenger
- Fare: Fare paid by the passenger
- Cabin: Cabin number of the passenger (Some entries contain NaN)
- Embarked: Port of embarkation of the passenger (C = Cherbourg; Q = Queenstown; S = Southampton)



Perguntas:
A partir dessas informações, é possível realizar alguns brainstormings sobre o acontecimento como:

- Quantos passageiros sobreviveram?
- Qual era a idade média? Qual era a idade do mais novo e do mais velho a sobreviver?
- Qual era o valor médio gasto em passagens dos sobreviventes?
- Mais mulheres ou homens sobreviveram ao acidente?
- Qual o percentual de sobreviventes por gênero?
- Qual o percentual de sobreviventes por classe social?
- Qual o percentual de sobreviventes por porto de embarque?
- Qual o percentual de sobreviventes que viajaram sozinhas e/ou com família?
- Qual a média de idade dos sobreviventes?
- De qual porto houve o maior número de passageiros?
- Qual o valor médio gasto por sexo, classe social e porto de embarque?
- Qual o % de sobrevivência entre crianças e adolescentes, adultos e idosos?
- Qual é a idade média dos sobreviventes por porto?

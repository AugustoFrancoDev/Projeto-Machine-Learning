# 🤖 Projeto de Análise, Limpeza e Modelagem Preditiva
Este é um repositório ao projeto de Ciência de Dados e Aprendizado de Máquina proposto na trilha de aprendizados do NIAD.

## 🎯 Objetivo do projeto
O projeto consistia em escolher entre três banco de dados, fazer limpezas desses dados, análise com representações visuais, então escolher o melhor modelo preditivo de acordo com as análises e
fazer uma análise dos resultados e importância das variáveis. Com este projeto, eu pretendia aprender e colocar em prática conhecimentos sobre estatística, ciência de dados e Machine Learning.

## 📁 Composição do repositório
O repositório em geral é bem simples. O arquivo [notaEstudos](notaEstudos.ipynb) é um notebook simples o qual eu utilizei para fazer algumas anotações iniciais. O arquivo [analiseReserva](analiseReserva.ipynb)
foi uma primeira tentativa de lidar com o banco de dados de terremotos. Mas como eu desisti desse banco de dados por não conseguir bons resultados logo no começo, mudei para o banco de dados de biometrias de
gambás, cuja análise geral está em [analiseGeral](analiseGeral.pynb), este é o arquivo principal deste repositório.

## 🛠️ Tecnologias e Ferramentas Utilizadas

**🧮 Manipulação e Matemática:**
**💻 Linguagem e Ambiente:**
* **[Python 3](https://www.python.org/):** Linguagem de programação base utilizada para toda a lógica e estruturação do projeto.
* **[Jupyter Notebook](https://jupyter.org/):** Ambiente de desenvolvimento interativo utilizado para a criação dos blocos de código, visualização instantânea dos gráficos e documentação narrativa da análise.

* **[Pandas](https://pandas.pydata.org/):** Utilizado para leitura, limpeza e estruturação do banco de dados em formato tabular (DataFrames).
* **[NumPy](https://numpy.org/):** Empregado para cálculos matemáticos avançados e operações com matrizes (como o cálculo do RMSE).

**📊 Visualização de Dados:**
* **[Matplotlib](https://matplotlib.org/):** Ferramenta base para a criação da estrutura, painéis e eixos dos gráficos.
* **[Seaborn](https://seaborn.pydata.org/):** Biblioteca construída sobre o Matplotlib para a plotagem de gráficos estatísticos mais avançados e com estética aprimorada.

**🧠 Machine Learning (Scikit-Learn):**
A biblioteca **[Scikit-Learn](https://scikit-learn.org/)** (ou `sklearn`) forneceu todo o motor preditivo e de validação do projeto, utilizando as seguintes ferramentas:
* **Modelos Preditivos:** `RandomForestRegressor` (algoritmo baseado em árvores de decisão) e `Ridge` (regressão linear com regularização matemática).
* **Preparação:** `train_test_split` para realizar a separação segura entre os dados de Treino e Teste.
* **Métricas de Avaliação:** `mean_squared_error` e `r2_score` para mensurar, respectivamente, a margem de erro absoluta em centímetros e a porcentagem de acerto do modelo.

## 🦘 Escolha do banco de dados
O banco de dados escolhido foi o de biometria de gambás. Como citado anteriormente, eu tentei trabalhar com o banco de dados de terremotos primeiro, mas por fim acabei optando por este.

## 🧗 Desafios e interpretação dos resultados do ao longo projeto
### 📓 Ambiente Jupyer
Não estava acostumado a utilizar os notebooks do ambiente Jupyter. Confesso que demorei um pouco até acostumar, mas uma vez que consegui me adaptar entendi porquê foi recomendado para o projeto e pretendo continuar utilizando,
é muito prático, útil e integra todas as ferramentas e tecnologias utilizadas.

### 🐍 Python
Embora eu já conhecesse um pouco da linguagem, fazia tempo que não a utilizava então precisei relembrar um pouco.

### 🧰 Outras ferramentas e bibliotecas
Os outros recursos eu consegui aprender a utilizar melhor colocando o conhecimento em prática.

### 🧹 Análise, limpeza e tipagem de dados
Para mim, esta foi a parte mais tranquila. Eu já entendia bem o conceito de preenchimento de valores nulos, conversão de tipos e lidar com *outliers*, então não senti muitos problemas.

### 🔍 Análise exploratória
Esta para mim foi a parte que eu subestimei e acabou se tornando a mais importante do projeto. Representações gráficas facilitam muito a visualização de padrões e correlações no banco de dados. Com essas informações,
podemos tomar decisões melhores para o melhor modelo preditivo a ser utilizado, portanto, esta parte acaba sendo o coração do projeto que define o rumo que ele irá tomar.

### ⚙️ Machine Learning: Implementação dos modelos preditivos
E foi aqui que eu tive as maiores dificuldades. Após testar alguns modelos preditivos, eu estava obtendendo c*oeficientes de determinação* baixos e tendo problemas com *overfitting*. Analisando melhor as possibilidades que 
eu tinha com as correlações do meu banco de dados, o melhor caminho parecia ser a implementação do modelo de *Regressão Ridge*. Mesmo assim, as métricas de de *coeficiente de determinação* e *RMSE* não foram tão satisfatórias,
e ainda tendo um gap bem considerável entre treinos e testes (evidência de *overfitting*). Acredito que pelo banco de dados ser relativamente pequeno (apenas 104 gambás), não seja possível conseguir métricas muito mais elevadas
do que essas, fora o fator de ser um banco de dados biométrico, área com muito mais variáveis e dificuldade de predição.

## 🏆 Conclusões finais
No fim, fico satisfeito com o projeto. Sinto que a trilha de aprendizado me introduziu e mudou minha visão sobre o que era Machine Learning e Ciência de Dados e estou bem interessado em continuar estudando e me aprofundando
nesses assuntos.

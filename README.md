# Simple-machine-learning

Importa a biblioteca pandas e a apelida como pd.
Usa a função pd.read_csv() para ler o arquivo "pizzas.csv".
O conteúdo do arquivo CSV é armazenado no DataFrame df, que é uma estrutura de dados semelhante a uma tabela, como as de bancos de dados ou planilhas do Excel.

O método .plot() gera gráficos diretamente a partir de um DataFrame do pandas.
Kind="scatter": define o tipo do gráfico como dispersão (scatter plot).
Cada ponto no gráfico representa um par (diametro, preco).
x="diametro", y="preco"

Define os eixos do gráfico:
Eixo X: diametro (tamanho da pizza).
Eixo Y: preco (valor da pizza).

Importa o módulo linear_model da biblioteca sklearn para trabalhar com modelos de regressão.
modelo = linear_model.LinearRegression(): cria uma instância do modelo de Regressão Linear, que será usado para encontrar a relação entre o diâmetro e o preço da pizza.
x = df[["diametro"]]
y = df[["preco"]]
x (variável independente): recebe a coluna "diametro" do DataFrame.
y (variável dependente): recebe a coluna "preco" do DataFrame.
As colunas são passadas dentro de [[]] para que os dados fiquem no formato correto (matriz de valores).
modelo.fit(x, y): treina o modelo com os dados (x e y).
O modelo aprende a relação entre o diâmetro da pizza e seu preço.

# Còdigo de execução do app
streamlit run app.py

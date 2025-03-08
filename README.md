## Simple machine learning
<div>A biblioteca pandas e a apelida como pd.
<div>Usa a função pd.read_csv() para ler o arquivo "pizzas.csv".
<div>O conteúdo do arquivo CSV é armazenado no DataFrame df, que é uma estrutura de dados semelhante a uma tabela, como as de bancos de dados ou planilhas do Excel.
</div>
  
<div>O método .plot() gera gráficos diretamente a partir de um DataFrame do pandas.
<div>Kind="scatter": define o tipo do gráfico como dispersão (scatter plot).
<div>Cada ponto no gráfico representa um par (diametro, preco).
<div>x="diametro", y="preco"
</div>
  
## Define os eixos do gráfico:
<div>Eixo X: diametro (tamanho da pizza).
<div>Eixo Y: preco (valor da pizza).
</div>
  
<div>Importa o módulo linear_model da biblioteca sklearn para trabalhar com modelos de regressão.
<div>modelo = linear_model.LinearRegression(): cria uma instância do modelo de Regressão Linear, que será usado para encontrar A relação entre o diâmetro e o preço da pizza.
<div>x = df[["diametro"]]
<div>y = df[["preco"]]
<div>x (variável independente): recebe a coluna "diametro" do DataFrame.
<div>y (variável dependente): recebe a coluna "preco" do DataFrame.
<div>As colunas são passadas dentro de [[]] para que os dados fiquem no formato correto (matriz de valores).
<div>modelo.fit(x, y): treina o modelo com os dados (x e y).
<div>O modelo aprende a relação entre o diâmetro da pizza e seu preço.
</div>

## Còdigo de execução do app
streamlit run app.py

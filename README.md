
# API para Regressão Linear

Essa API foi construída utilizando o pacote `plumber` e tem como
objetivo aplicar regressão linear em um conjunto de dados previamente
existente. A API também oferece funcionalidades para adicionar,
modificar e deletar registros, fazer predições com base no modelo
treinado e gerar gráficos e análises estatísticas.

# Endpoints

## POST /registro

Adiciona um novo registro ao conjunto de dados.

**Parâmetros:**

- x: Valor do parâmetro x.
- grupo: Valor do parâmetro grupo.
- y: Valor da variável dependente y.

## DELETE /deletar_registro

Deleta um registro da tabela de dados, especificando a linha.

**Parâmetros:**

- l: Número da linha a ser deletada.

## POST /modificar_registro

Modifica um registro existente na tabela de dados.

**Parâmetros:**

- l: Número da linha a ser modificada.
- x: Novo valor do parâmetro x.
- grupo: Novo valor do parâmetro grupo.
- y: Novo valor do parâmetro y.

## GET /grafico

Gera um gráfico mostrando a relação entre x, y e grupo com ajuste de uma
regressão linear.

## GET /residuos

Retorna os resíduos do modelo ajustado.

## GET /plot_residuos

Gera gráficos dos resíduos padronizados, histograma e Q-Q plot.

## GET /significancia

Retorna a tabela de coeficientes com significância estatística.

## POST /predicao

Recebe uma lista em formato JSON com novos dados e retorna as predições.

**Parâmetros:**

- string: JSON contendo x e grupo para realizar predições.
"# APIreg" 

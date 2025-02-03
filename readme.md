# Projeto de Ciência de dados 
## Previsão de score bancário
### Feramentas exploradas:

- Python
    - 
    - Jupter
- Análise de Dados 
    - 
    - Pandas
- Machine Learning 
    -
    - Sklearn
    - Random Forest
    - KNeighbors

## Descrição do Código:
O código "main.ipynb" importa os dados presente na tabela "clientes.csv", em seguida realiza o pré-processamento, eliminando colunas com linhas vazias e codificando strings em valor númericos.

Após essa etapa, os dados são separaos em X e Y, o primeiro os valores para serem analisados e o segundo o valor que se busca prever

Ambos, são dividos em X_treino, X_teste, Y_treino e Y_teste. Os valores com o sufixo "treino" foram usados para treinar os modelos de machine learng e os com "teste" para calcular a precisão das IA.

Foram feitos teste no modelo RandomForest e KNeighbors e após a acurácia o modelo RandomForest obteve melhor aproveitamento nessa base de dados.

Agora, com o modelo de IA já criado e selecionado, os dados da tabela "novos_clientes.csv" passaram pelo mesmo pré-processamento.

Por fim, foi usado o modelo de machine learng criado para prever o score de crédito (Y), dos novos clientes, obtendo como resultado: 'Poor', 'Good', 'Good'.
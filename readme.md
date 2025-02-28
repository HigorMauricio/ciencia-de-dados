# Projeto de Ciência de dados 
## Previsão de score bancário
### Feramentas exploradas:

- Python
    - 
    - Jupyter
- Análise de Dados 
    - 
    - Pandas
- Machine Learning 
    -
    - Sklearn
    - Random Forest
    - KNeighbors

## Descrição do Código:
### Importação e visuazalição no Pandas
O código "main.ipynb" importa os dados presente na tabela "clientes.csv", em seguida realiza o pré-processamento, eliminando colunas com linhas vazias e codificando strings em valor númericos.

- Tabela clientes.csv:

![Image](https://github.com/user-attachments/assets/111e11f7-3f76-4626-a371-dba06750133c)
*Ao todo são 25 colunas e 100000 linhas*


- Pré-Processamento:

![Image](https://github.com/user-attachments/assets/86a27031-5eb4-4fc0-9871-2e934f400b3e)
*Coluna de ID removida e dados do tipo str alterados para int*


### Preparação 

Após essa etapa, os dados são separaos em X e Y, o primeiro são os valores para serem analisados e o segundo o valor que se busca prever

Ambos, são dividos em X_treino, X_teste, Y_treino e Y_teste. Os valores com o sufixo "treino" foram usados para treinar os modelos de machine learng e os com "teste" para calcular a precisão das IA.

![Image](https://github.com/user-attachments/assets/11b19c44-e8f3-47df-9e7d-4030ac5b82a3)


### Criação da IA
Foram feitos teste no modelo RandomForest e KNeighbors e após a acurácia o modelo RandomForest obteve melhor aproveitamento nessa base de dados.

- Criação:

![Image](https://github.com/user-attachments/assets/33a5c8ed-a022-4032-b014-0ebbaaaef030)
*Foi criado o modelo RandomForest e  KNeighbors*

- Acurácia:

![Image](https://github.com/user-attachments/assets/76ccefb4-5757-46c8-96d2-09e5e301b53b)
*Modelo RandomForest se mostrou melhor então foi o selecionado*


### Utilização para novos clientes

Agora, com o modelo de IA já criado e selecionado, os dados da tabela "novos_clientes.csv" passaram pelo mesmo pré-processamento.

Por fim, foi usado o modelo de machine learng criado para prever o score de crédito (Y), dos novos clientes, obtendo como resultado: 'Poor', 'Good', 'Good'.

![Image](https://github.com/user-attachments/assets/254f8d25-7ce8-48ac-85ad-0c851afdea3c)
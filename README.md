# Inteligencia artificial com Lógica Fuzzy no Mercado
Lógicas fuzzy permitem a associação entre dados númericos e conhecimento qualitativo com palavras que expressam faixas de interesse.
Esse é um projeto de introdução que utilizou como **Input** o RSI (Relative Strength Index e do Volume relativo de negociação do BOVA11, para relacionar os conceitos, regras,
**"Baixo","Médio" e "Alto"** dos valores dos indicarores ee ter como **Output** a decisão de **"Comprar", "Manter" ou "Vender"** BOVA11. \

O Modelo implementado resultou nos sinais abaixo:
![image](https://github.com/caiomferreira/Fuzzy/blob/e9b8c43abe814a5a9c9cd7a9ef309de40ade0fe2/Resultado%20L%C3%B3gica%20Fuzzy.png)
 - Não é indicação de Investimento.

## As regas abaixo descrevem o sistema de controle fuzzy utilizado tomar as decisões.
- Regra 1: Se o RSI estiver baixo e o Volume Relativo estiver baixo, então a decisão é comprar. \
- Regra 2: Se o RSI estiver baixo e o Volume Relativo estiver médio, então a decisão é comprar. \
- Regra 3: Se o RSI estiver baixo e o Volume Relativo estiver alto, então a decisão é comprar. \
- Regra 4: Se o RSI estiver médio e o Volume Relativo estiver alto, então a decisão é manter. \
- Regra 5: Se o RSI estiver médio e o Volume Relativo estiver médio, então a decisão é manter. \
- Regra 6: Se o RSI estiver alto e o Volume Relativo estiver baixo, então a decisão é manter. \
- Regra 7: Se o RSI estiver alto e o Volume Relativo estiver médio, então a decisão é vender. \
- Regra 8: Se o RSI estiver alto e o Volume Relativo estiver alto, então a decisão é vender. \
- 
com elas podemos criar funções de pertinência, atribuir um peso para cada Input e gerar um Output sendo o que melhor se adequa as regras criadas. \
_____________
abaixo imagem do universo decisão

![image](https://github.com/caiomferreira/Fuzzy/blob/e9b8c43abe814a5a9c9cd7a9ef309de40ade0fe2/universo%20decis%C3%A3o.png)



### Foi utilizada a Biblioteca SciKit-Fuzzy
https://pythonhosted.org/scikit-fuzzy/overview.html

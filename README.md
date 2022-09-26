<p align="center"><strong>
ANÁLISE EXPLORATÓRIA DE DADOS E CLASSIFICAÇÃO DE SOBREVIVENTES COM ÁRVORE DE DECISÃO
</strong></p>
<hr style="margin-bottom: 40px;">


&nbsp;

## Titanic

<img align="right" alt="Titanic" height="300" style="border-radius:50px;" src="https://github.com/Mariana-Alvim/Arvore-de-Decisao/blob/main/Imagens/Titanic.jpg"></img>

O próposito deste algoritmo foi classificar usando um modelo de Machine Learning a chance de um passageiro sobreviver ao Titanic conforme seu gênero, idade, classe econômica, número e parentesco dos acompanhantes e local de embarque.

Além disso, buscou-se obter insights explorando as relações entre as variáveis explicativas e a variável resposta.


O conjunto de dados do Titanic foi importado diretamente da biblioteca seaborn. Ele contém 891 observações (dos quais 342 ou 38%  são sobreviventes).

Por meio do modelo de classificação foi obtida uma acurácia de 82% no conjunto de treino e 78% no conjunto de teste. </body>

 
&nbsp;

&nbsp;

## O modelo de Árvore de Decisão

A árvore de decisão é um algoritmo supervisionado de Machine Learning usado para classificação. A árvore de decisão é construída por meio da partição recursiva binária. Ou seja, ela consiste em divisões sucessivas em duas partes cada vez que é identificada uma diferenciação a partir das variáveis explicativas que aumente o poder preditivo.

As divisões ou quebras são chamadas de nós e conduzem à predições cada vez melhores. O critério da diferenciação é aquele que gera a menor impureza ou maior homogeneidade da variável resposta. Resumindo, o algoritmo visa minimizar a impureza em cada quebra. 

Nesse trabalho, foi utilizado o índice Gini para selecionar e ordenar as variáveis explicativas conforme a maior redução de impureza . O Índice de Gini é uma métrica de impureza e seu valor varia de 0,0 a 0,5. A acurácia aumenta conforme diminui a impureza ou quanto mais próximo de 0,0 for o índice de Gini. Se o índice Gini for 0,0 significa que todas as predições estarão corretas.    

Como hiperparâmetro (parâmetro de controle do algoritmo para reduzir a chance de ocorrer overfitting), foi utilizada uma profundidade máxima da árvore igual a 3. Ademais, como método de cross-validation, foi utilizada a separação do conjunto de dados em conjunto de treino e conjunto de teste. Então, o conjunto de treino foi utilizado para treinar o modelo, enquanto o conjunto de teste foi usado para avaliar o modelo. 


![Fluxograma](https://github.com/Mariana-Alvim/Arvore-de-Decisao/blob/main/Imagens/Fluxograma.png)

 
&nbsp;
 
&nbsp;
&nbsp;

&nbsp;

* ### Equação de determinação do Índice de Gini
<p align="center"><img src="https://github.com/Mariana-Alvim/Arvore-de-Decisao/blob/main/Imagens/%C3%8Dndice%20de%20Gini.png"
    style="width:600px; float: left; margin-left: 50%; display: flex;"></img></p>

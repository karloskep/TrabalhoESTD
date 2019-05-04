## Problema 1 
>###### Quais são as duas características mais comuns para analisar algoritmos?
As duas características mais comuns para analisar um software para dizer se é bom ou ruim são: Tempo e Consumo de memória.

## Problema 2 
>###### Por que a medida de tempo em segundos não representa qualificadamente o tempo de execuçãoo de um algoritmo?
Não é medida em tempo o software já que deve possuir certa independência entre a tecnología; o software e o hardware.

## Problema 3 
>###### A medida de tempo de um algoritmo é realizada através de qual informação? O que pode afetá-la?
A medição do tempo em representação a qualidade e estabilidade do software é feita mediante os passos do algoritmo que precisa para finalizar a sua execução.
Pode afetá-la pelo ambiente do hardware em que ela é executada e o tamanho da entrada.

## Problema 4 
>###### Na análise de algoritmos, qual é o valor da base da função logarítmica e exponencial? Por que é escolhido este valor?
A base da função logarítmica e exponencial é 2.
A base 2 tem uma importância muito considerada na informática dada a codificação binária que utiliza. O número determinado em um bit é de oito (8) exemplares que podem codificar-se com 2^8 = 256 que é o número de variações que pode realizar-se.
O algoritmo binário tem uma frequência de aparição grande no análise de algoritmos.

## Problema 5 
>###### O que é complexidade de tempo?
É uma função que representa o número máximo de passos de um algoritmo.

## Problema 6 
>###### Dado dois algoritmos A e B com as complexidades de tempo respectivamente f1 e f2, qual é o melhor algoritmo? O que indica qual é o melhor algoritmo?
Considerando A e B dois algoritmos totalmentes diferentes, é selecionado o melhor aquele que é executado com menores números de passos à finalização da execução e aquele que tem uma menor complexidade de tempo.

## Problema 7 
>###### Em uma função de complexidade, o que representa o termo n?
Em uma função de complexidade o termo “n” é considerado como o comprimento da entrada.

## Problema 8 
>###### Quais são as operações primitivas de um algoritmo?
As operações primitivas de um algoritmo são:
- Atribuição de valores a variáveis;
- Chamadas de métodos;
- Operações aritméticas;
- Comparação de dois números;
- Acesso a um arranjo;
- Seguimento de uma referência para um objeto;
- Retorno de um método.

## Problema 9 
>###### Qual é o valor de uma operação primitiva de um algoritmo?
Para cada valor de uma operação primitiva de um algoritmo é atribuído o valor 1.

## Problema 10 
>###### Desenvolva o pseudocódigo do algoritmo SOMA, que realiza a soma de dois números inteiros recebidos por parâmetro e tem como saída a resultado da operação. Identifique a sua função de complexidade de tempo.
```
1 - p <- a + b
2 - retorna p;
```
Sendo custo c1 e c2;
<br />
f(n) = c1 . 1 + c2 . 1
<br />
f(n) = 1 + 1
<br />
f(n) = 2

## Problema 11 
>###### Desenvolva o pseudocódigo do algoritmo SOMA VETOR, que realiza a soma de todos os elementos de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua função de complexidade de tempo.
```
1 - soma <- 0;
2 - N <- comprimento V;
3 - para i <- 1 até N:
4 -        soma <- soma + V[i]
5 -        i <- i + 1
6 - retorna soma;
```
Sendo custo c1, c2, c3, c4, c5 e c6, o número de vezes no para(for) assume o valor de n, então:
<br />
f(n) = c1 . 1 + c2 . 1 + c3 . n + c4 . n + c5 . n + c6 . 1
<br />
f(n) = 1 + 1 + n + n + n + 1
<br />
f(n) = 3n + 3

## Problema 12
>###### Desenvolva o pseudocódigo do algoritmo CONTAGEM IMPARES, que realiza a contagem de números impares de um vetor. O algoritmo recebe o vetor V e tem como saída o resultado. Identifique a sua função de complexidade de tempo.
```
1 - cont <- 0;
2 - N < comprimento V;
3 - para i <- 1 até N:
4 -        se V[i]%2 != 0:
5 -           cont <- cont + 1
7 -        i <- i + 1
8 - retorna cont;
```
Sendo custo c1, c2, c3, c4, c5, c6 e c7, o número de vezes no para(for) e se(if) assume o valor de n, então:
<br />
f(n) = c1 . 1 + c2 . 1 + c3 . n + c4 . n + c5 . n + c6 . n + c7 . 1
<br />
f(n) = 1 + 1 + n + n + n + n + 1
<br />
f(n) = 4n + 3

## Problema 13
>###### Desenvolva o pseudocódigo do algoritmo SOMA MATRIZ, que realiza a soma de todos os elementos de uma matriz. O algoritmo recebe a matriz M e tem como saída o resultado. Identifique a sua função de complexidade de tempo.
```
1 - soma <- 0;
2 - N <- comprimento M;
3 - para i <- até N:
4 -        para j <- 1 até N:
5 -             soma <- soma + M[i][j]
6 -             j <- j + 1
7 -        i <- i + 1
8 - retorna soma;
```
Sendo custo c1, c2, c3, c4, c5, c6, c7 e c8, o número de vezes no para(for) assume o valor de n, para o para(for) dentro do outro para(for), o número de vezes assume o valor de n . n, então:
<br />
f(n) = 1 + 1 + n + n * n + n * n + n * n + n + 1
<br />
f(n) = 3n² + 2n + 3

## Problema 14
>###### Desenvolva o pseudocódigo do algoritmo BUSCA MATRIZ, que identifica posiçãoo x e y de um elemento em uma matriz. O algoritmo recebe a matriz M e o valor V e tem como saída a posição x e y . Identifique a sua funçao de complexidade de tempo.
```
1 - N <- comprimento M;
2 - para i <- 1 até N:
3 -        para j <- 1 até N:
4 -             se M[i][j] = V:
5 -                retorna M[i][j];
6 -             j <- j + 1
7 -        i <- i + 1
8 - retorna M;
```
Sendo custo c1, c2, c3, c4, c5, c6, c7 e c8, o número de vezes no para(for) assume o valor de n, para o para(for) dentro do outro para(for) e o se(if), o número de vezes assume o valor de n . n, então:
<br />
f(n) = 1 + n + n² + n² + n² + n² + n + 1
<br />
f(n) = 4n² + 2n + 2

## Problema 15
>###### O que é análise assintótica? Qual é o seu objetivo?
A análise assintótica é um método de descrever o comportamento de limites, com objetivo de compreender o tempo de execução para entradas grandes.

## Problema 16 
>###### Qual é o processo da análise assintótica? Crie um exemplo

1 - f(n) = 6n³ + 2n² + 20n + 45;
<br />
2 - Identificar o componente de maior ordem;
<br />
3 - 6n³;
<br />
4 - Ignorar os coeficientes;
<br />
5 - n³;
<br />
Dizemos que f é assintoticamente no, máximo, n³.

## Problema 17 
>###### O que é a notação assintótica?
É uma notação utilizada para descrever o relacionamento é f(n) = O(n³).

## Problema 18 
>###### O que é a notação O-Grande ou Big-Oh?
Notação O-Grande diz que uma função é menor que ou igual a outra função g(n). Ou seja, f é limitada superiormente por g assintoticamente. Geralmente é usada para mostrar como os programas precisam de recursos em relação ao tamanho de entrada.

## Problema 19 
>###### Qual é a definição formal da notação O-Grande?
Formalmente definimos como: Onde R+ é o conjunto dos reais não negativos.

## Problema 20 
>###### Crie um gráfico explicando a notação O-grande. Utilize f(n) = 2n + 4. Qual é um valor possível para n0?
![questao20](https://raw.githubusercontent.com/gherickds/AnaliseAlgoritmosESTD/master/big-oh.PNG)
<br />
Possível valor para n0:
<br />
n0 = 4
## Problema 21 
>###### O que é a notação o-pequeno ou Little-Oh?
É uma notação a qual diz que uma função é menor que a outra g(n). Ou seja, f é dominada por g assintoticamente.

## Problema 22 
>###### Qual é a definição formal da notação o-pequeno?
Formalmente definimos como: Onde R+ é o conjunto dos reais não negativos.

## Problema 23 
>###### Crie um gráfico explicando a notação o-pequeno.
![questao23](https://raw.githubusercontent.com/gherickds/AnaliseAlgoritmosESTD/master/little-oh.PNG)
## Problema 24 
>###### Passe a notação O-grande e o-pequeno as funções abaixo:
**A) F(n) = n + 1**
<br />
O-grande(n)
<br />
o-pequeno(n²)

**B) F(n) = 8**
<br />
O-grande(1)
<br />
o-pequeno(n)

**C) F(n) = 2n² − 1**
<br />
O-grande(n²)
<br />
o-pequeno(2^n)

**D) F(n) = nlogn**
<br />
O-grande(logn)
<br />
o-pequeno(n²)

**E) F(n) = 3n! + 2n**
<br />
O-grande(n!)
<br />
o-pequeno(n!²)

**F) F(n) = 3n³ + 2n² + 4n + 6**
<br />
O-grande(n³)
<br />
o-pequeno(n!)

**G) F(n) = 5^n + 11**
<br />
O-grande(5^n)
<br />
o-pequeno(n * n!)

**H) F(n) = 3logn**
<br />
O-grande(logn)
<br />
o-pequeno(n²)

## Problema 25 
>###### Identifique o O-Grande dos algoritmos desenvolvidos nos Problemas 10 até 14.
**10- f(n)=2**
<br />
O-grande(1)

**11- f(n)=3n+3**
<br />
O-grande(m)

**12- f(n)=4n+3**
<br />
O-grande(n)

**13- f(n)=3n² + 2n + 3**
<br />
O-grande(n²)

**14- f(n)=4n² + 2n + 2**
<br />
O-grande(n²)

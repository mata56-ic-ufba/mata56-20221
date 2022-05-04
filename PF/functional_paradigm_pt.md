# The Functional Paradigm

<!-- 
Neste capítulo, apresentamos as principais propriedades da programação funcional. 
Na programação funcional, a computação procede reescrevendo funções e não modificando o estado. 
A característica fundamental das linguagens nesse paradigma, pelo menos em sua forma “pura”, 
é justamente a de não possuir o conceito de memória (e, portanto, efeitos colaterais). 
Uma vez que um ambiente é definido, uma expressão sempre denota o mesmo valor.
Discutiremos o paradigma puro nas primeiras seções, explicando os aspectos fundamentais. 
As linguagens de programação funcionais, no entanto, mesclam esses ingredientes “puros” em um contexto que adiciona 
outros mecanismos; vamos revisá-los na Sec. 11.3.
Abordaremos a máquina SECD, uma máquina abstrata para linguagens funcionais de ordem superior (higher-order)
que constitui o protótipo de muitas implementações reais. 
Estaremos, neste ponto, em condições de discutir as razões pelas quais o paradigma de programação funcional 
é interessante em relação às linguagens imperativas comuns. 
O capítulo termina com uma seção mais teórica que fornece uma introdução sucinta ao λ-calculus, 
um sistema formal de computabilidade que inspira todas as linguagens funcionais e que tem sido, 
desde a época de ALGOL e LISP, um modelo constante para o projeto de linguagens de   programação.
--> 

## 11.1 Computações sem estado

Todas as linguagens convencionais baseiam seu modelo computacional no conceito de transformação do estado.
O coração deste modelo é o conceito de variável modificável, ou seja, um container com um nome ao qual
podem ser atribuídos valores diferentes, enquanto a mesma associação nome-container é sempre mantida no ambiente.
Analogamente, a principal construção em linguagens convencionais é o comando de atribuição, que modifica o valor (r-value)
guardado em uma variável, mas não modifica a associação entre o nome da variável e a localização a que corresponde (l-value).

```
l-value = r-value
```

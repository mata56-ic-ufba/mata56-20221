# O Paradigma Funcional

<!--
## Visão geral
### Computação com "State" (Imperative)
+ state, (modifiable) variable, assignment, l-value, r-value, iteration
+ computational model: transformation of state
+ von Neumann's machine
-->

## 11.1 Computação sem "Estado"
+ rewriting expressions
+ higher-order functions, recursion
+ computational model: "stateless", transformation of environment

### Linguagens Funcionais

+ Puras: LISP, Miranda, Haskell
+ Scheme, ML

### Expressões

## 11.2 Avaliação

## 11.3 Programação Funcional

+ local environment
+ interactiveness
+ types
+ pattern matching
+ infinite objects
+ aspectos imperativos

## 11.4 Máquinas Abstratas

## 11.5 Avaliação

## 11.6 Lambda-calculus


An abstract model for characterising computable functions based on higher-order functions and recursion.


## Resumo

+ _Abstraction_. A mechanism for passing from one expression denoting a value to one denoting a function.
+ _Application_. A mechanism dual to abstraction, by which a function is applied to an argument.
+ _Computation_ by rewriting or reduction, in which an expression is repeatedly simplified until a form that can not be further reduced is encountered.
+ _Redex_. The syntactic structure which is simplified during reduction and is formed from the application of an abstraction to an expression.
+ The centrality of _higher order_ in this mode of computation.

# O Paradigma Funcional

<!-- 
In this chapter, we present the main properties of functional programming. 
In functional programming, computation proceeds by rewriting functions and not by mod ifying the state. 
The fundamental characteristic of the languages in this paradigm, at least in their “pure” form, 
is precisely that of not possessing the concept of memory (and therefore side effect). 
Once an environment is fixed, an expression always denotes the same value. 
We will discuss the pure paradigm in the first sections, explaining the funda mental aspects. 
Functional programming languages, however, merge these “pure” ingredients in a context that adds many other mechanisms; 
we will review them in Sect. 11.3. 
We will touch on the SECD machine, an abstract machine for higher-order functional languages 
which constitutes the prototype of many real implementations. 
We will, at this point, be in a position to discuss the reasons why the functional programming paradigm 
is interesting with respect to ordinary imperative languages. 
The chapter concludes with a more theoretical section which provides a succinct introduction to the λ-calculus, 
a formal system for computability which inspires all functional languages and which has, 
since the time of ALGOL and LISP, been a constant model for the design of programming languages. 
–>

## 11.1 Computations without State 

Though developed and abstract, all conventional languages base their computational model on the transformation of the state. 
The heart of this model is the concept of modifiable variable, that is, a container with a name to which, during the computation, 
can be assigned different values, while the same association is always main tained in the environment. 
Correspondingly, the principal construct in conventional languages is assignment, which modifies the value contained in a variable 
(but does not modify the association between the name of the variable and the location to which it corresponds; 
it modifies the r-value but not the l-value, which is fixed once and for all when the variable is declared). 

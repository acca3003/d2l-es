# Notación
:label:`chap_notation`

A lo largo de este libro, seguiremos las siguientes convenciones de notación.
Tener en cuenta que alguno de estos símbolos son marcadores, mientras otros 
se refieren a objetos específicos.
Como regla general, el artículo indefinido "un/una" indica
que el símbolo es un marcador y que símbolos similarmente formateados
pueden denotar otros objetos del mismo tipo.
Por ejemplo, "$x$: un escalar" significa
que las letras minúsculas generalmente representan valores escalares.


## Objetos Numéricos

* $x$: un escalar
* $\mathbf{x}$: un vector
* $\mathbf{X}$: una matriz
* $\mathsf{X}$: un tensro genérico
* * $\mathbf{I}$: una matriz identidad---cuadrada, con $1$ en todos los elementos de la diagonal y $0$ en todos los elementos fuera de la diagonal
* $x_i$, $[\mathbf{x}]_i$: el $i^\mathrm{th}$ elemento del vector $\mathbf{x}$
* $x_{ij}$, $x_{i,j}$,$[\mathbf{X}]_{ij}$, $[\mathbf{X}]_{i,j}$: el elemento de la matriz $\mathbf{X}$ en la fila $i$ y columna $j$.



## Teoría de Conjuntos


* $\mathcal{X}$: un conjunto
* $\mathbb{Z}$: el conjuntos de los números enteros
* $\mathbb{Z}^+$: el conjunto de los números enteros positivos
* $\mathbb{R}$: el conjunto de los números reales
* $\mathbb{R}^n$: el conjunto vecotres $n$-dimensionales de números reales
* $\mathbb{R}^{a\times b}$: El cojunto de matrices de números reales con $a$ filas y $b$ columnas
* $|\mathcal{X}|$: cardinalidad (número de elementos) de un conjunto $\mathcal{X}$
* $\mathcal{A}\cup\mathcal{B}$: union de los conjuntos $\mathcal{A}$ y $\mathcal{B}$
* $\mathcal{A}\cap\mathcal{B}$: intersección de los cojuntos $\mathcal{A}$ y $\mathcal{B}$
* $\mathcal{A}\setminus\mathcal{B}$: conjunto substracción de $\mathcal{B}$ a $\mathcal{A}$ (contiene sólo aquellos elementos de $\mathcal{A}$ que no pertenecen a $\mathcal{B}$)



## Funciones y Operadores


* $f(\cdot)$: a function
* $\log(\cdot)$: the natural logarithm (base $e$)
* $\log_2(\cdot)$: logarithm with base $2$
* $\exp(\cdot)$: the exponential function
* $\mathbf{1}(\cdot)$: the indicator function, evaluates to $1$ if the boolean argument is true and $0$ otherwise
* $\mathbf{1}_{\mathcal{X}}(z)$: the set-membership indicator function, evaluates to $1$ if the element $z$ belongs to the set $\mathcal{X}$ and $0$ otherwise
* $\mathbf{(\cdot)}^\top$: transpose of a vector or a matrix
* $\mathbf{X}^{-1}$: inverse of matrix $\mathbf{X}$
* $\odot$: Hadamard (elementwise) product
* $[\cdot, \cdot]$: concatenation
* $\|\cdot\|_p$: $\ell_p$ norm
* $\|\cdot\|$: $\ell_2$ norm
* $\langle \mathbf{x}, \mathbf{y} \rangle$: dot product of vectors $\mathbf{x}$ and $\mathbf{y}$
* $\sum$: summation over a collection of elements
* $\prod$: product over a collection of elements
* $\stackrel{\mathrm{def}}{=}$: an equality asserted as a definition of the symbol on the left-hand side



## Calculus

* $\frac{dy}{dx}$: derivative of $y$ with respect to $x$
* $\frac{\partial y}{\partial x}$: partial derivative of $y$ with respect to $x$
* $\nabla_{\mathbf{x}} y$: gradient of $y$ with respect to $\mathbf{x}$
* $\int_a^b f(x) \;dx$: definite integral of $f$ from $a$ to $b$ with respect to $x$
* $\int f(x) \;dx$: indefinite integral of $f$ with respect to $x$



## Probability and Information Theory

* $X$: a random variable
* $P$: a probability distribution
* $X \sim P$: the random variable $X$ has distribution $P$
* $P(X=x)$: the probability assigned to the event where random variable $X$ takes value $x$
* $P(X \mid Y)$: the conditional probability distribution of $X$ given $Y$
* $p(\cdot)$: a probability density function (PDF) associated with distribution P
* ${E}[X]$: expectation of a random variable $X$
* $X \perp Y$: random variables $X$ and $Y$ are independent
* $X \perp Y \mid Z$: random variables  $X$  and  $Y$ are conditionally independent given $Z$
* $\sigma_X$: standard deviation of random variable $X$
* $\mathrm{Var}(X)$: variance of random variable $X$, equal to $\sigma^2_X$
* $\mathrm{Cov}(X, Y)$: covariance of random variables $X$ and $Y$
* $\rho(X, Y)$: the Pearson correlation coefficient between $X$ and $Y$, equals $\frac{\mathrm{Cov}(X, Y)}{\sigma_X \sigma_Y}$
* $H(X)$: entropy of random variable $X$
* $D_{\mathrm{KL}}(P\|Q)$: the KL-divergence (or relative entropy) from distribution $Q$ to distribution $P$



[Discussions](https://discuss.d2l.ai/t/25)

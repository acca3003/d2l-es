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
* $\mathbf{I}$: una matriz identidad---cuadrada, con $1$ en todos los elementos de la diagonal y $0$ en todos los elementos fuera de la diagonal
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


* $f(\cdot)$: una función
* $\log(\cdot)$: el logaritmo neperiano/natural (base $e$)
* $\log_2(\cdot)$: logaritmo con base $2$
* $\exp(\cdot)$: la función exponencial
* $\mathbf{1}(\cdot)$: la función indicador, evalua a $1$ si el argument booleano es verdadero y a $0$ en cualquier otro caso
* $\mathbf{1}_{\mathcal{X}}(z)$: la función indicador de miembro de un conjunto, evalua a $1$ si el elemento $z$ pertenece al conjunto $\mathcal{X}$ y $0$ en cualquier otro caso
* $\mathbf{(\cdot)}^\top$: transposición de un vector o matriz
* $\mathbf{X}^{-1}$: inversa de una matriz $\mathbf{X}$
* $\odot$: producto Hadamard (por elementos)
* $[\cdot, \cdot]$: concatenación
* $\|\cdot\|_p$: $\ell_p$ norma
* $\|\cdot\|$: $\ell_2$ norma
* $\langle \mathbf{x}, \mathbf{y} \rangle$: producto escalar/punto de los vectores $\mathbf{x}$ y $\mathbf{y}$
* $\sum$: suma de una colección de elementos
* $\prod$: producto de una colección de elementos
* $\stackrel{\mathrm{def}}{=}$: una igualdad afirmada como una definición a la izquierda del símbolo



## Cálculo

* $\frac{dy}{dx}$: derivada de $y$ respecto a $x$
* $\frac{\partial y}{\partial x}$: derivada parcial de $y$ respecto a $x$
* $\nabla_{\mathbf{x}} y$: gradiente de $y$ respecto a $\mathbf{x}$
* $\int_a^b f(x) \;dx$: integral definida de $f$ entre $a$ y $b$ con respecto a $x$
* $\int f(x) \;dx$: integral indefinida def $f$ respecto a $x$



## Probabilidad y Teoría de la Información

* $X$: una variable aleatoria
* $P$: una distribución de probabilidad
* $X \sim P$: la variable aleatoria $X$ con distribución $P$
* $P(X=x)$: la probabilidad de que la variable aleatoria $X$ tome el valor $x$
* $P(X \mid Y)$: distribución de la probabilidad condicional $X$ dado $Y$
* $p(\cdot)$: una función de densidad (PDF) associated with distribution P
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

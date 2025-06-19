# Álgebras de Hopf Trenzadas sobre Grupos Finitos no Abelianos


En el estudio de álgebras de Hopf y sus representaciones,
la categoría de módulos de Yetter–Drinfeld juega un rol central.
Estos objetos surgen naturalmente en contextos como la teoría de
trenzados, la construcción del doble de Drinfeld y la clasificación
de álgebras de Hopf de dimensión finita. En esta exposición nos
enfocaremos en la categoría de módulos de Yetter–Drinfeld sobre
un álgebra de grupo, es decir, sobre $H = \Bbbk G$, donde $G$
es un grupo finito y $\Bbbk$ un cuerpo algebraicamente cerrado
cuya característica no divide el orden de $G$.

La categoría ${}_H^H \mathcal{YD}$ de módulos de Yetter–Drinfeld
sobre $H = \Bbbk G$ resulta ser semisimple bajo estas hipótesis,
y admite una descripción explícita y elegante de sus objetos
simples en términos de datos combinatorios y representacionales
asociados al grupo $G$: clases de conjugación y representaciones
irreducibles de subgrupos isotropía. Esta descripción se puede
encontrar en trabajos como los de Andruskiewitsch y Graña,
donde se formaliza la construcción de los módulos simples mediante
inducción desde representaciones de subgrupos centrales, y se prueba
que toda clase de isomorfismo de objeto simple en
${}_H^H \mathcal{YD}$ aparece de esta manera.

En esta nota seguiremos este enfoque y desarrollaremos en detalle
los siguientes aspectos:

- Definiremos la categoría de módulos de Yetter-Drinfeld
sobre un álgebra de grupo $\Bbbk G$, es decir, daremos la
caracterización explícita de sus objetos y morfismos.
- Mostraremos que un objeto $M$ de ${}_H^H \mathcal{YD}$
equivale a un $G$-módulo graduado por $G$, es decir, una
descomposición $M = \bigoplus_{g \in G} M_g$ compatible con la
acción de $G$ de modo que $g \cdot M_h \subseteq M_{ghg^{-1}}$
para todo $g,h \in G$.
- Presentaremos la construcción de los objetos simples
$M(g,\rho)$ a partir de una clase de conjugación $\mathcal{O}_g$
y una representación irreducible $\rho$ del subgrupo centralizador
$\Gamma_g$, siguiendo la [Definición~3.1.1](https://arxiv.org/abs/math/9802074v3) de
Andruskiewitsch-Graña.
- Demostraremos la [Proposición~3.1.2](https://arxiv.org/abs/math/9802074v3): que todo
objeto simple de ${}_H^H \mathcal{YD}$ es isomorfo a uno de los
$M(g,\rho)$, y que estos forman una familia de representantes no
isomorfos.
- Consideraremos el caso en que $G$ es abeliano, donde la
categoría toma una forma especialmente sencilla, descrita en el
[Corolario~3.1.3.](https://arxiv.org/abs/math/9802074v3)
- Finalmente, utilizaremos GAP para  dar una descripción
completa de los objetos simples en ${}_H^H \mathcal{YD}$
cuando $G = \mathbb{S}_3$, el grupo simétrico de tres
elementos, determinando todos los posibles pares
$(g,\rho)$ que dan lugar a objetos simples.


El objetivo es presentar estos resultados con el grado de
detalle necesario para su comprensión rigurosa, haciendo
énfasis en las construcciones explícitas, los cálculos y
las ideas detrás de las pruebas.

## Conexión al repo

```
echo "# hopfalg" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/juniors90/hopfalg.git
git push -u origin main
```
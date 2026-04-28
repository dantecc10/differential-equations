# Ecuaciones Diferenciales con Transformada de Laplace
## Mtro. Luis Enrique Aguilar Morales
### Dante Castelán Carpinteyro


El operador de la _*Transformada de Laplace*_ se denota de la siguiente manera:

$\mathcal{L} \\{\\}$

La fórmula de la Transformada de Laplace es $\mathcal{L} \{f(t)\} = \int_{-\infty}^{\infty} f(t)e^{-st}dt$.

$s$ es otra variable.

$\mathcal{L} \\{f(t)\\} = \int_{0}^{\infty} f(t)e^{-st}dt$ $\to$ causales.

si $f(t) = c = 1$ para $\mathcal{L} \\{1\\} = \int_{0}^{\infty} 1e^{-st}dt = - \frac{1}{s} \cdot e^{-st}|_{0}^{\infty}$*.

*Lo que sea $\neq t$ es considerado una constante.

Esto se evalúa como $[- \frac{1}{s} \cdot e^{-s \cdot \infty}] - [- \frac{1}{s} \cdot e^{-s \cdot 0}] = [- \frac{1}{s \cdot e^{s \cdot \infty}}] - [- \frac{1}{s \cdot e^{s \cdot 0}}]$.

Aplicando las potencias a los exponenciales:

$[- \frac{1}{s \cdot e^{\infty s}}] - [- \frac{1}{s \cdot e^{0}}] = [- \frac{1}{s \cdot e^{\infty}}] - [- \frac{1}{s \cdot 1}] = [- \frac{1}{s \cdot \infty}] - [- \frac{1}{s}] = [- \frac{1}{\infty}] - [- \frac{1}{s}] = [- (0)] - [- \frac{1}{s}] = - [- \frac{1}{s}] = \frac{1}{s}$

Con esto, se obtiene $\frac{1}{s}$ como resultado de una función $f(t) = 1$ pasado por el operador de la Transformada de Laplace. Este al ser lineal, permite plantear lo siguiente:

$\mathcal{L} \\{1\\} = \frac{1}{s} \therefore \mathcal{L} \\{k\\} = k \cdot \mathcal{L} \\{1\\} = \frac{k}{s}$

Y, considerando el operador inverso de la Transformada de Laplace:

$\mathcal{L}^{-1} \\{\frac{1}{s}\\} = 1$ y $\mathcal{L}^{-1} \\{\frac{k}{s}\\} = k$.

Ahora, para una función $f(t) = t$ el desarrollo sería:

$\mathcal{L} \\{f(t)\\} = \int_{0}^{\infty} t \cdot e^{-st} dt$.

Desarrollamos la integral:

$\int_{0}^{\infty} t \cdot e^{-st} dt$, donde aplicaré una integración por partes con variables:

Sea $\int u \cdot dv = u \cdot v - \int v \cdot du$, tomando las siguientes variables:

$(u = t) \therefore (du = dt)$

$(dv = e^{-st}) \therefore (v = \int dv = - \frac{1}{s} \cdot e^{-st})$

Aplicando la fórmula:

$\int u \cdot dv = u \cdot v - \int v \cdot du \to \int_{0}^{\infty} t \cdot e^{-st} = t \cdot (- \frac{1}{s} \cdot e^{-st}) - \int_{0}^{\infty} (- \frac{1}{s} \cdot e^{-st}) \cdot dt$

<div align="left">
$$
[(- \frac{t}{s} \cdot e^{-st})]|_{0}^{\infty} - [\int_{0}^{\infty} (- \frac{1}{s} \cdot e^{-st}) \cdot dt]
$$
</div>

$[(- \frac{\infty}{s} \cdot e^{-s \cdot \infty}) - (- \frac{0}{s} \cdot e^{-s \cdot 0})] - [(- \frac{1}{s}) \cdot \int_{0}^{\infty} e^{-st} \cdot dt]$

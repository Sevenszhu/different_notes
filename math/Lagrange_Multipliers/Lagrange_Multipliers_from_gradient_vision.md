# View Lagrange Multipliers in a Gradient Vision

> This article focuses on understanding in Lagrange Multipliers how Lagrange function
is derived with parallel of two functions' (original function and constraint function) gradients.
Providing a specific perspective, it will help green hands to Lagrange Multipliers easier to 
construct connection between gradients and the method.

## Problem: an original function in the constraint of another function
We want to minimize:
f(x,y)=x^2+y^2

x+y=2.

## Method: Lagrange Multipliers

## Lagrange Multiplier Method

$$
\begin{aligned}
\min_{x,y}\quad & f(x,y)=x^2+y^2\\
\text{s.t.}\quad & x+y=2
\end{aligned}
$$

$$
\mathcal L(x,y,\lambda)=x^2+y^2-\lambda(x+y-2)
$$

$$
\begin{cases}
\displaystyle\frac{\partial\mathcal L}{\partial x}=2x-\lambda=0\\[8pt]
\displaystyle\frac{\partial\mathcal L}{\partial y}=2y-\lambda=0\\[8pt]
\displaystyle\frac{\partial\mathcal L}{\partial\lambda}=-(x+y-2)=0
\end{cases}
$$

$$
\begin{cases}
2x=\lambda\\
2y=\lambda\\
x+y=2
\end{cases}
$$

$$
2x=2y\implies x=y
$$

$$
x+y=2\implies 2x=2\implies x=1
$$

$$
y=1,\qquad\lambda=2
$$

$$
\mathcal L(x,y,2)
=(x-1)^2+(y-1)^2+2\ge 2
$$

$$
\boxed{(x^*,y^*)=(1,1)}
$$

$$
\boxed{f_{\min}=f(1,1)=2}
$$


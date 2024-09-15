# Equacions diferencials de 1r ordre
Una ==equació diferencial ordinària de primer ordre== per a una funció $y(x)$ és una equació 
$$F(x,y(x), y'(x)) = 0$$

La forma explícita d'una *edo* de 1r ordre és 
$$
\frac{dy}{dx} = y'(x) = f(x,y(x)) \text{ o (*)} f(x,y)
$$
L'equació (\*) es diu ==autònoma== si $f$ no depèn explícitament de $x$. O sigui, és de la forma 
$$\begin{align*}
y' &= f(y) \\
( y'(x) &= f(y(x)) ) 
\end{align*}$$
Una solució de (\*) és una funció $y(x)$ és una funció diferenciable definida en un interval $I$ tal que per tot $x \in I$ satisfà (\*)

```ad-example
La funció $y(x) = e^x +x + 1$ és solució de l'equació $y' = y - x$ $$e^x + 1 = e^x + x + 1 - x$$ De fet, $y(x) = \alpha e^x + x + 1$ és solució $\forall \alpha \in \mathbb{R}$
```

En general, les solucions d'una edo de 1r ordre formen una família uniparamètrica de funcions depenent d'un paràmetre constant. Aquesta expressió s'anomena ==solució general de la edo== de 1r ordre.

```ad-example
La família uniparamètrica $y(x) = c e^x$ és solució de l'edo $y' = y$
```

````ad-definition
Una equació diferencial de 1r ordre amb una condició inicial s'anomena ==problema de valor inicial== $$\begin{cases}
y' &= f(x,y) \\
y(x_0) &= y_{0}
\end{cases}$$
La solució d'un problema de valor inicial s'anomena ==solució particular de l'equació==
````

Un cas particular de solucions són els ==equilibris==, que són les solucions que no depenen de la variable independent (de $x$).
Una solució d'equilibri de $y' = f(x,y)$ és una solució de la forma $y(x) = y* \text{(numero)}$. Es compleix que $y(x)=y*$ és solució d'equilibri de $$y' = f(x,y) \iff f(x,y*)=0$$ per tot $x$ per al qual $f(x,y)$ estigui ben definit.

Si l'equació és autònoma $y' = f(y)$ les solucions d'equilibri $y(x) = y*$ estan donades pels zeros de $f$ i estan definides $\forall x \in \mathbb{R}$

```ad-example
 1) $y' = (y-1)e^x$  --> $f(x) = 1$
 2) $y' = y - x$ --> No té equilibri
```


## Existència, Unitat i Continuïtat de Solucions

````ad-theorem
title: Teorema *(Picard - Cindelof)*

Sigui $R$ una regió regular del pla $xy$ definida per $R= \{(x,y) \mid a \le x \le b, \, c \le y \le d\}$, que conté el punt $(x_0, y_0)$.
Suposem que $f$ i que $\frac{\partial f}{\partial y}$ sigui continues a $R$. Aleshores existeix uns única solució $y(x)$ definida a un interval $I_0 = (x_o - h, x_0 + h), \, h > 0$ contingut a $[a, b]$ del problema de valor inicial (PVI)
$$(*)\begin{cases}y' = f(x,y) \\y(x_0) = y_0\end{cases}$$
A més a més si denotem la solució de (\*) per $y(x; x_0, y_0)$ es compleix que $y(x; x_0, y_0)$ és una funció continua respecte $x_0$, $y_0$

Existència $\implies f$ contínua (Peano)
Per assegurar unicitat és suficient amb que $f$ sigui de **Lipschitz** respecte la variable $y$. És a dir: $$\exists L > 0 \text{ (constant) t.q. } |f(x,y)-f(x,z)| < L|y-z| \, \forall y,z \in (c,d)$$
````

````ad-theorem
Si $f$ i $\frac{\partial f}{\partial y}$ són contínues a $\mathbb{R}$ aleshores dues corbes solució de $y' = f(x,y)$ diferents no es poden tallar a $\mathbb{R}$.
````

````ad-example
$$\begin{cases}
y' = \sqrt{|y(x)|} \\
y(0) = 0
\end{cases}$$
Les funcions $y_1(x) = 0$ i $y_{2} = \begin{cases}
+\frac{x^2}{4} &\text{ si } x \ge 0 \\
-\frac{x^2}{4} &\text{ si } x < 0
\end{cases}$
````

## Alguns mètodes analítics de resolució
### EDOS Separables o de variables separades
Una edo de variables separada és de la forma $$y' = g(x) \cdot h(y)$$ 
Si $h(y) = 0$, $\frac{1}{h(y)} y'(x) = g(x)$. Integrant respecte $x$ tenim 
$$\int \frac{1}{h(y(x))}y'(x) dx = \int g(x) dx$$
Denotem per $H$ una primitiva de $\frac{1}{h(y)}$ i per $G$ una primitiva de $g(x)$
$$
\begin{align*}
H(y(x)) &= G(x) + C \\
\frac{1}{h(g(x))} &= g(x)
\end{align*}
$$
Per tant $H(y(x)) - G(x) = C$.

````ad-example
<u>Llei de refredament de Newton</u>
Velocitat de refredament d'una substància és proporcional a la diferència de temperatura de la substància i l'ambient.
Si la temperatura ambient és de 30ºC i la substància es refreda de 1000ºC a 70ºC en 15min, en quin moment estarà a 40ºC?  -> T(t) = 40

$$\begin{cases}
T'(t) = \alpha(T(t) - T_0) \\
T(0) = 1000 \\
T(15) = 70

\end{cases}$$
$$\begin{align*}
\frac{dT}{dt} &= \alpha(T - 30) \\
\int \frac{dT}{T - 30} &= \int \alpha \, dt \\
\ln |T - 30| &= \alpha t + C\\
|T - 30| &= e^{\alpha t} e^{C}\\
T - 30 &= \mathcal{C} e^{\alpha t}\\
T(t) &= 30 + \mathcal{C} e^{\alpha t}
\end{align*}$$
````

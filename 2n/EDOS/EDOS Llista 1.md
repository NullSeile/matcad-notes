`````ad-exercice
title: **1. Vegeu si les següents funcions, o famílies de funcions, són solució de la corresponent equació diferencial:**



````ad-exercice
title: **a) $\bm{x(t) = 2e^{-2t} + \frac{1}{3}e^t}$, $\bm{x' + 2x = e^t}$**

$$
x' = -4e^{-2t} + \frac{1}{3}e^t
$$
Calculem $x' + 2x$:
$$\begin{align*}
x' + 2x &= -4e^{-2t} + \frac{1}{3}e^t + 4e^{-2t} + \frac{2}{3}e^t \\
&= e^t
\end{align*}$$

````

````ad-exercice
title: **b) $\bm{x(t) = e^{-t} \cos(\frac{t}{2})}$, $\bm{x'' + x' = e^{-t} \cos\left(\frac{t}{2}\right)}$**
$$\begin{align*}
x'(t) &= -e^{-t} \left(\cos\frac{t}{2} + \frac{1}{2} \sin\frac{t}{2}\right) \\
x''(t) &= e^{-t} \left( \frac{3}{4} \cos \frac{t}{2} + \sin \frac{t}{2} \right)
\end{align*}$$

$$\begin{align*}
x'' + x' &= \frac{3}{4} e^{-t} \cos \frac{t}{2} + e^{-t} \sin \frac{t}{2} - e^{-t} \cos \frac{t}{2} - \frac{1}{2} e^{-t} \sin \frac{t}{2} \\
&= -\frac{1}{2} e^{-t} \cos \frac{t}{2} + \frac{1}{2} e^{-t} \sin \frac{t}{2} \\
&= \frac{1}{2} e^{-t} \left(\sin\frac{t}{2} - \cos\frac{t}{2}\right) = e^{-t} \cos \frac{t}{2} \\
&\iff \sin \frac{t}{2}- \cos \frac{t}{2} = 2 \cos \frac{t}{2} \iff \sin \frac{t}{2} = 3 \cos \frac{t}{2}
\end{align*}$$
````

````ad-exercice
title: **c) $\bm{x(t) = t \tan t}$, $\bm{t x' = x + t^2 + x^2}$**
$$x'(t) = \frac{t}{\cos^2 t} + \tan t = \frac{t}{\cos^2 t} + \frac{\sin t}{\cos t} = $$
```handwritten-ink
{
	"versionAtEmbed": "0.2.6",
	"filepath": "Ink/Writing/2024.9.17 - 20.54pm.writing"
}
```
````
````ad-exercice
title: **d) $\bm{x(t) = c_1 + c_2 e^{-t} + \frac{t^3}{3}}$, $\bm{x'' + x' = t^2 + 2t}$**
```handwritten-ink
{
	"versionAtEmbed": "0.2.6",
	"filepath": "Ink/Writing/2024.9.17 - 21.16pm.writing"
}
```

````
`````

`````ad-exercice
title: **2. Per a cada equació diferencial i família de corbes, comproveu si les corbes de la família són solució de l'equació diferencial. En cas afirmantiu, trobeu quina corba de la família satisfà les condicions inicials**

````ad-exercice
title: **a) $\bm{x·x' + 6t = 0}$, $\bm{x^2 = -6t^2 + c}$; $\bm{x(0) = 4}$**

$$\begin{align*}
x^2 &= -6t^2 + c \\
x &= \pm\sqrt{-6t^2 + c}\\
x' &= \frac{-6t}{\pm\sqrt{-6t^2 + c}}
\end{align*}$$
Comprovem si l'equació és solució de l'equació diferencial:
$$\begin{align*}
x·x' + 6t &= \pm\sqrt{-6t^2 + c} · \frac{-6t}{\pm\sqrt{-6t^2 + c}} + 6t \\
&= -6t + 6t = 0
\end{align*}$$

Ara busquem la corba que satisfà la condició inicial:
$$\begin{align*}
x(0) = 4 &\implies 4^2 = c \implies c = 16 \\
x &= \sqrt{-6t^2 + 16}
\end{align*}$$
````

````ad-exercice
title: **b) $\bm{x' = 1 + x^2}$, $\bm{x = \tan(t+c)}$; $\bm{x\left(\frac{\pi}{4}\right)= 1}$**

```handwritten-ink
{
	"versionAtEmbed": "0.2.6",
	"filepath": "Ink/Writing/2024.9.17 - 21.36pm.writing"
}
```
````

````ad-exercice
title: **c) $\bm{x·x' = e^{2t} + 1}$, $\bm{x^2 = e^{2t} + 2t + c}$; $\bm{x(0) = \frac{1}{2}}$**
```handwritten-ink
{
	"versionAtEmbed": "0.2.6",
	"filepath": "Ink/Writing/2024.9.17 - 21.45pm.writing"
}
```
````

````ad-exercice
title: **d) $\bm{2x'' + x' - x = 0}$, $\bm{x = c_1 e^{\frac{t}{2}} + c_2 e^{-t}}$; $\bm{x(0) = 0}$, $\bm{x'(0) = 1}$**

$$\begin{align*}
x' &= \frac{c_1}{2} e^{\frac{t}{2}} - c_2 e^{-t} \\
x'' &= \frac{c_1}{4} e^{\frac{t}{2}} + c_2 e^{-t}
\end{align*}$$
```handwritten-ink
{
	"versionAtEmbed": "0.2.6",
	"filepath": "Ink/Writing/2024.9.17 - 21.49pm.writing"
}
```
````

`````

`````ad-exercice
title: **3. $\bm{x' = 3x^{\frac{2}{3}}}$ té infinites solucions satisfent $\bm{x(0) = 0}$.**
$$
x'(t) = 3x^{\frac{2}{3}} = g(t)·h(x)
$$
Amb $g(t) = 1$ i $h(x) = 3x^{\frac{2}{3}}$.
$$
\frac{\partial x}{\partial t} = 3x^{\frac{2}{3}} \iff \frac{\partial x}{3x^{\frac{2}{3}}} = \partial t \iff \frac{3}{3}x^{\frac{1}{3}} = t + c \iff \frac{1}{3} \int x^{-\frac{2}{3}} dx = \int \partial t
	$$
`````



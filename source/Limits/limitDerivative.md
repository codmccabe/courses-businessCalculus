# Limit Definition of the Derivative

#### Recall (Average Rate of Change)

The average rate of change of $f$ over the interval $[a,b]$ or slope
of the secant line to the graph of $f$ through the points $(a,f(a))$
and $(b,f(b))$ is
$$
\frac{f(b)-f(a)}{b-a}.
$$

However, in order to get the instantaneous rate of change $b-a=0$ or $b=a$ and that is impossible to calculate using the average rate of change expression. This is sensical because the average rate of change is meant to calculate average rate of change and no instantaneous rate of change. In order to find the instantaneous rate of change we must evaluate the expression $\dfrac{f(b)-f(a)}{b-a}$ as $b$ approaches $a$. The limit will help us calculate this situation.

The instantaneous rate of change of $f$ at $a$ or the slope of the
tangent line to the graph of $f$ at $(a,f(a))$ is

$$
\lim_{b\to a}\frac{f(b)-f(a)}{b-a}.
$$

![secant2tangent1.svg](attachment:secant2tangent1.svg)

![secant2tangent2.svg](attachment:secant2tangent2.svg)

If we let $x$ be a starting point (the point we desire the tangent
slope), and $b=x+h$ where $h\ne0$. Then 

$$
x\to b\implies h\to0
$$

and we can write the following 

$$
\begin{aligned}m=\lim_{x\to b}\frac{f(b)-f(x)}{b-x} & =\lim_{h\to 0}\frac{f(x+h)-f(x)}{(x+h)-x}\\
 & =\lim_{h\to 0}\frac{f(x+h)-f(x)}{h}.
\end{aligned}
$$

Given any value $x$ in the point where one wants the tangent slope
(instantaneous rate of change). An operation needed to find
the tangent slope would be to evaluate
$$
\lim_{h\to0}\frac{f(x+h)-f(x)}{h}.
$$

---
#### Example
Find the average rate of change and instantaneous rate of change to the function $f(x)=x$ from $x=1$ to $x=2$. Next, find the instantaneous rate of change to the function at $x=1$ and at $x=2$.


**Solution**:

To find the average rate of change we have:

$$
\dfrac{f(2)-f(1)}{2-1}=\dfrac{2-1}{2-1}=1
$$

This is as expected since $f$ is a linear function with a slope of $1$.

Next, attempt to find the instantaneous rate of change of $f$ at $x=1$. This means we must attempt to evaluate the following limit:

$$
\lim_{h\to 0}\dfrac{f(x+h)-f(x)}{h}=\lim_{h\to0}\dfrac{(x+h)-x}{h}
$$

when $x=1$. That is:

$$
\begin{align*}
\lim_{h\to0}\dfrac{f(1+h)-f(1)}{h} & =\lim_{h\to0}\dfrac{(1+h)-(1)}{h}\\
 & =\lim_{h\to0}\dfrac{h}{h}\\
 & =\lim_{h\to0}1\\
 & =1
\end{align*}
$$

Next, attempt to find the instantaneous rate of change of $f$ at
$x=2$. This means we must attempt to evaluate the following limit:

$$
\lim_{h\to0}\dfrac{f(x+h)-f(x)}{h}
$$

when $x=2$. That is:

$$
\begin{align*}
\lim_{h\to0}\dfrac{f(2+h)-f(2)}{h} & =\lim_{h\to0}\dfrac{(2+h)-(2)}{h}\\
 & =\lim_{h\to0}\dfrac{h}{h}\\
 & =\lim_{h\to0}1\\
 & =1
\end{align*}
$$

Recap, 

* the average rate of change of the function $f$ over the interval $[1,2]$ is $1$.
* The instantaneous rate of change of the function $f$ exactly at $x=1$ is $1$.
* The instantaneous rate of change of the function $f$ exactly at $x=2$ is $1$.

---
The action of finding the rate of change at an exact point on a curve is called differentiation. For example, in Newtonian physics an object in free fall in a vacuum is:

$$
f(x)=-9.8 x
$$

The instantaneous rate of change of an object in free fall is the rate of change in $f$ at some value $x$. In order to find the instantaneous rate of change (or velocity) of $f$ at some $x$ value we need the derivative the action of differentiation.

#### Definition (The Limit Definition of the Derivative)
The derivative of a function $f$ with respect to $x$ is the function
$f'$ "$f$ prime'',
$$
f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h}.
$$
The set of all $x$ such that $f'(x)$ exists is the domain of $f'(x)$
or the set of $x$ where $f$ is differentiable.

---

Common notations that are used to represent derivatives are: $f'(x)$, $\frac{dy}{dx}$, and $y'$ to list a few.

#### Example
Find the instantaneous rate of change (or derivative) of the function

$$
f(x)=x^2 + x + 1
$$

at $x=1$.

SOLUTION:

Here we want to evaluate 
$$
\lim_{h\to0}\dfrac{f(x+h)-f(x)}{h}
$$
when $x=1$. That is, we want to evaluate
$$
\lim_{h\to0}\dfrac{f(1+h)-f(1)}{h}
$$

First, we will identify $f(1+h)$
$$
\begin{align*}
f(1+h) & =(1+h)^{2}+(1+h)+1\\
 & =1+2h+h^{2}+1+h+1\\
 & =h^{2}+3h+3
\end{align*}
$$
Second, we will simplify $f(1+h)-f(1)$
$$
\begin{align*}
h^{2}+3h+3-(1^{2}+1+1) & =h^{2}+3h+3-3\\
 & =h^{2}+3h
\end{align*}
$$
Third, we will simplify $\dfrac{f(1+h)-f(1)}{h}$
$$
\begin{align*}
\dfrac{h^{2}+3h}{h} & =\dfrac{h(h+3)}{h}\\
 & =h+3
\end{align*}
$$
Finally, we will evaluate $\lim_{h\to0}\dfrac{f(1+h)-f(1)}{h}$
$$
\lim_{h\to0}(h+3)=0+3=3
$$

Therefore, the instantaneous rate of change of the function $f$ at
$x=1$ is $3$. Alternatively, we can say
$$
f'(1)=3
$$

It is common to find the derivative as a function. Then we will use that derivative function to find several instantaneous rate of changes or describe behaviors of the original function.

#### Example
Use the limit definition of the derivative to find the derivative of the function
$$
f(x)=4x^2-5x+1
$$

SOLUTION:

We want to find
$$
f'(x)=\lim_{h\to0}\dfrac{f(x+h)-f(x)}{h}
$$

First, we will find $f(x+h)$
$$
\begin{align*}
f(x+h) & =4(x+h)^{2}-5(x+h)+1\\
 & =4\left(x^{2}+2xh+h^{2}\right)-5(x+h)+1\\
 & =4x^{2}+8xh+4h^{2}-5x-5h+1\\
 & =4\,x^{2}+8\,h\,x-5\,x+4\,h^{2}-5\,h+1
\end{align*}
$$
Second, we will simplify $f(x+h)-f(x)$
$$
\begin{align*}
f(x+h)-f(x) & =4\,x^{2}+8\,h\,x-5\,x+4\,h^{2}-5\,h+1-\left(4x^{2}-5x+1\right)\\
 & =8\,h\,x+4\,h^{2}-5\,h
\end{align*}
$$
Third, we will simplify $\dfrac{f(x+h)-f(x)}{h}$
$$
\begin{align*}
\dfrac{f(x+h)-f(x)}{h} & =\dfrac{8hx+4h^{2}-5h}{h}\\
 & =\dfrac{h(8x+4h-5)}{h}\\
 & =8x+4h-5
\end{align*}
$$
Finally, hit is with the limit
$$
\lim_{h\to0}\left(8x+4h-5\right)=8x+4(0)-5=8x-5.
$$

Therefore, the function that provides the instantaneous rate of change
for any input $x$ is
$$
f'(x)=8x-5
$$
where the original function if $f(x)$.

#### Example
Use the limit definition of the derivative of the function
$$
f(x)=\dfrac{1}{\sqrt{x}}
$$

SOLUTION:

We want to find 
$$
f'(x)=\lim_{h\to0}\dfrac{f(x+h)-f(x)}{h}
$$

First, we will find $f(x+h)$
$$
f(x+h)=\dfrac{1}{\sqrt{x+h}}
$$

Second, we will simplify $f(x+h)-f(x)$
$$
\begin{align*}
f(x+h)-f(x) & =\dfrac{1}{\sqrt{x+h}}-\dfrac{1}{\sqrt{x}}\\
 & =\dfrac{\sqrt{x}-\sqrt{x+h}}{\sqrt{x}\sqrt{x+h}}\cdot\left(\dfrac{\sqrt{x}+\sqrt{x+h}}{\sqrt{x}+\sqrt{x+h}}\right)\\
 & =\dfrac{x-(x+h)}{\sqrt{x}\sqrt{x+h}\left(\sqrt{x}+\sqrt{x+h}\right)}\\
 & =\dfrac{-h}{\sqrt{x}\sqrt{x+h}\left(\sqrt{x}+\sqrt{x+h}\right)}
\end{align*}
$$
Third, we will simplify $\dfrac{f(x+h)-f(x)}{h}$
$$
\begin{align*}
\dfrac{f(x+h)-f(x)}{h} & =\dfrac{\dfrac{-h}{\sqrt{x}\sqrt{x+h}\left(\sqrt{x}+\sqrt{x+h}\right)}}{h}\\
 & =\dfrac{-h}{\sqrt{x}\sqrt{x+h}\left(\sqrt{x}+\sqrt{x+h}\right)}\cdot\dfrac{1}{h}\\
 & =\dfrac{-1}{\sqrt{x}\sqrt{x+h}\left(\sqrt{x}+\sqrt{x+h}\right)}
\end{align*}
$$
Finally, hit it with the limit
$$
\begin{align*}
\lim_{h\to0}\dfrac{-1}{\sqrt{x}\sqrt{x+h}\left(\sqrt{x}+\sqrt{x+h}\right)} & =\dfrac{-1}{\sqrt{x}\sqrt{x+0}\left(\sqrt{x}+\sqrt{x+0}\right)}\\
 & =-\dfrac{1}{x\left(2\sqrt{x}\right)}\\
 & =-\dfrac{1}{2x\sqrt{x}}
\end{align*}
$$
Therefore, the derivative of the function $f(x)=\dfrac{1}{\sqrt{x}}$
is
$$
f'(x)=-\dfrac{1}{2x\sqrt{x}}.
$$

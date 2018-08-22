---
title: 'Intuition in Calculus: Getting Intimate with The Power Rule'
date: 2018-08-20
permalink: /posts/2018/08/The_Power_Rule/
tags:

---

Learning about derivatives in Calculus I, I was really questioning why the power rule ‘worked’. Why is

$$\frac{d}{dx}(x^3) = 3x^2$$?

 Why do we multiply by 3?  In other words, why is

$$\frac{d}{dx}(x^n) = nx^{n-1}$$?

To answer this question let's start off with one of the easiest non-trivial derivatives to find: one of a straight line -

$$y = \color{orange}m\color{black}x + b$$

The derivative is obviously $\color{orange}m$, as that’s the slope of the line for all *x*. We learned that in middle school! It makes sense, as the ‘$\frac{dy}{dx}$’ is defined as rate of change in *y* over rate of change of *x*. For every time *x* increases by 1, *y* increases by m. In other words, for

$$ y = \color{orange}2\color{black}x + 3$$

The rate of change of *y* relative to *x* (or $\frac{dy}{dx}$) is $\color{orange}2$. We can see this using this chart:

| *x* | *y*  | Change in *x* from previous     | change in *y* from previous    |
|---|----|-------------|--------------|
| 1 | 5  | (initial value) | (initial value) |
| 2 | 7  |              +1 |  +2 |
| 3 | 9  |               +1|  +2|
| 4 | 11 |             +1|  +2|


* We know $y$ increases by 2 for every increase in $x$ by one. This is because $x$’s coefficient is $\color{orange}2$. Increasing $x$ from 3 to 4 brought us from having three $\color{orange}2$’s to having four $\color{orange}2$’s. (Going back to second grade, multiplication is just how many times you add something!)

* Generalizing this, We can say derivative of a linear functions $f(x)$ is just the coefficient of $x$, or $\color{orange} m$.

However, this doesn’t tell us how to find the derivative of a power two or greater. Lets use our previous example of $x^3$, and **incorrectly** apply our ‘coefficient rule’.

$$\frac{d}{dx} (x^3) = \frac{d}{dx} (x \cdot x \cdot x) = \frac{d}{dx} (\color{orange}{x^2} \cdot \color{black}x) $$

$$ = \color{orange}{x^2}$$

So our derivative would seemingly be $\color{orange}{x^2}$, as that's our coefficient of $x$.

We know that's not correct, as the derivative of $x^3$ is actually $3x^2$. Why? **It’s because we’re not increasing one $x$ by one, but instead we’re increasing every $x$ by one. We have three $x$’s, and each of their coefficients are $x^2$ (the other two $x$’s).**

In other words, we have (enumerating each *x* with subscripts)

$$ f(x) = \color{red}{ x_1} \color{black} \cdot \color{green}{x_2} \color{black} \cdot \color{blue}{ x_3}$$

When we increase $\color{red} {x_1}$ by one, we have an additional ‘$\color{green}{x_2} \color{blue}{ x_3}$’ for the same reason we had an additional ‘2’ in our linear equation 2.

However, we are increasing all $x$’s in $f(x)$ by one, not just $\color{red}{x_1}$. Since $\color{green}{x_2}$ is also being increased when we increase $x$ by one, it's the equivalent of it's coefficent of $\color{red}{x_1} \color{blue}{x_3}$ being added. Likewise, when $\color{blue}{x_3}$ increased by one, it's like adding $\color{red}{ x_1} \color{green}{ x_2}$. In other words:

Coefficients of $\color{red}{x_1}$ :

$$ f(x) = \color{red}{x_1} \color{black} \cdot \color{orange}{ (x_2 \cdot \color{orange}x_3)}$$

Coefficients of $\color{green}{x_2}$ :

$$ f(x) = \color{orange}{ (x_1)} \color{black} \cdot \color{green} {x_2} \color{black} \cdot \color{orange}{ (x_3)}$$

Coefficients of $\color{blue}{x_3}$:

 $$ f(x) = \color{orange} {(x_1  \cdot  \color{orange} x_2)} \color{black}\cdot \color{blue}{ x_3}$$




Because we are increasing ***every*** $x$ by one, $f(x)$ is increased by the coefficient of every $x$ (and that means counting coefficents multiple times)

$$ \color{green}{ x_2} \color{blue}{x_3} \color{black} + \color{red}{x_1} \color{blue}{x_3} \color{black} + \color{red}{ x_1} \color{green}{x_2} $$

Or

$$ 3x^2$$
 



Other people have described it in a similar way, but I like my description better. Hopefully this helps someone!

If you want to ask a question, tell me why I'm wrong, or just discuss the weather feel free to email me: ```lastnamefirstinitial@etsu.edu```
Fill in my last name and first initial obviously (to prevent spam).




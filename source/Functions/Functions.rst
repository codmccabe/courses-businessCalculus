.. code:: maxima

    set_plot_option([svg_file, "maxplot.svg"])$

Review of Functions
===================

This is a quick run through of functions.

Definition of Function
^^^^^^^^^^^^^^^^^^^^^^

A function :math:`f` is a rule of correspondence that associates with
each element :math:`x` in one set :math:`D`, called the domain, a single
value of :math:`f(x)` from a second set, :math:`R`. The set of all
values obtained is called the range of the function.

--------------

Functions by Names
------------------

Linear Function
^^^^^^^^^^^^^^^

A function whose graph is described as a line is called a linear
function. Algebratically denoted

.. math:: f(x)=mx+b=a_1 x + a_0

To expand from the previous definition we recall the following important
definition.

Definition of Polynomials
^^^^^^^^^^^^^^^^^^^^^^^^^

A function :math:`P` is called a polynomial if

.. math::


   P(x)=a_{n}x^{n}+a_{n-1}x^{n-1}+\cdots+a_{2}x^{2}+a_{1}x+a_{0}

where :math:`n` is a non-negative integer and the numbers
:math:`a_{0},a_{1},...,a_{n}` are constants called the coefficients of
the polynomial. The domain of any polynomial is
$:raw-latex:`\mathbb{R}`=:raw-latex:`\left`{
x,|,x:raw-latex:`\in`(-:raw-latex:`\infty`,:raw-latex:`\infty`):raw-latex:`\right`}
$. If the leading coefficient :math:`a_{n}\ne0`, then the degree of the
polynomial is :math:`n`.

Power Function
^^^^^^^^^^^^^^

A function of the form

.. math:: f(x)=x^a

where :math:`a` is a real number is called a power funciton. \* If
:math:`a=1,2,3,...` we have a polynomial. \* If :math:`a=\frac{1}{n}`
where :math:`n=1,2,3,...`, then we say

.. math:: f(x)=x^{\frac{1}{n}}=\sqrt[n]{x}

\ is a root function. \* If :math:`n` is even then the domain of
:math:`f` is :math:`\{x|x\in[0,\infty)\}`. \* If :math:`n` is odd then
the domain of :math:`f` is :math:`\{x|x\in(-\infty,\infty)\}`. \* If
:math:`a=-1,-2,-3,...`, then we say

.. math:: f(x)=x^a=\frac{1}{x^{-a}}

is the reciprocal function. \* If :math:`a=-1`, then we have

.. math:: f(x)=x^{-1}=\frac{1}{x^{-(-1)}}=\frac{1}{x^1}=\frac{1}{x}

\* If :math:`a=0`, then we say

.. math:: f(x)=x^0=1

is the constant function.

Absolute Value Function
^^^^^^^^^^^^^^^^^^^^^^^

The absolute value function is

.. math::


   |x|=\begin{cases}
   x & \text{if} x\ge 0\\
   -x & \text{if} x<0
   \end{cases} = \sqrt[2]{x^2}

Expoential Function
^^^^^^^^^^^^^^^^^^^

A function of the form :math:`f(x)a^x`, where :math:`a>0` and
:math:`a\ne 1`, is called an exponential function with base :math:`a`.
The domain of the exponential function is
:math:`\{ x | x\in (-\infty,\infty) \}` and the range is
:math:`\{ y | y\in (0,\infty) \}`.

.. code:: maxima

    plot2d([exp(x),exp(-x)],[x,-5,5],[y,-1,5],[legend,"f(x)=e^x","f(x)=e^{-x}"]);



.. image:: output_2_0.svg


Logarithmic Function
^^^^^^^^^^^^^^^^^^^^

A function of the form :math:`f(x)=\log_{a}(x)`, where :math:`a\ne1` and
:math:`a>0`, is called a logarithmic function “log base a of x”. The
domain of the logarithmic function is :math:`\{ x | x\in (0,\infty) \}`
and the range of :math:`\{ y | y\in(-\infty,\infty) \}`.

.. math:: y=a^x \iff x=\log_a(y)

.. code:: maxima

    plot2d([log(x),log(-x)],[x,-5,5],[y,-5,5],[legend,"y=ln(x)","y=ln(-x)"]);


.. parsed-literal::

    plot2d: expression evaluates to non-numeric value somewhere in plotting range.
    plot2d: expression evaluates to non-numeric value somewhere in plotting range.



.. image:: output_4_1.svg


# Partial-derivatives-and-differentiation-

## ( 3.5 ) Partial derivatives of composite functions : change of variables , ( 3.6) Partial differentiation of implicit functions ##

---

### 3.5 PARTIAL DIFFERENTIATION OF COMPOSITE FUNCTIONS: CHANGE OF VARIABLES

In the study of heat equation, wave equation, and Laplace’s equation, it is very often required to transform the representing partial differential equations in Cartesian coordinate system to cylindrical, spherical, or orthogonal curvilinear systems by changing the variables through partial differentiation of composite functions (function of a function).

Let \( u = f(x, y, z) \) and \( x, y, z \) are functions of two (or more) independent variables, say \( s \) and \( r \) as \( x = x(s, t), y = y(s, t), z = z(s, t) \). Then \( f \) is considered as a function of \( s \) and \( t \) via the intermediate variables \( x, y, z \). Now the derivative of \( u \) w.r.t. \( t \) is partial but not total. Keeping \( s \) constant, Equation (3) is modified as:

\[
\left(\frac{\partial r}{\partial t}\right)_s = \frac{\partial x}{\partial t} \frac{\partial f}{\partial x} + \frac{\partial y}{\partial t} \frac{\partial f}{\partial y} + \frac{\partial z}{\partial t} \frac{\partial f}{\partial z} \tag{5}
\]

The subscript \( s \) in (5) indicates the variable which is held constant. With this convention \( \left(\frac{\partial f}{\partial t}\right)_s \) may be written as \( \frac{\partial f}{\partial t} \) and so on. However, following the convention that \( \frac{\partial f}{\partial t} \), without subscripts, indicates the result of differentiating \( f \) w.r.t. the explicitly appearing variable \( x \), while holding all other explicitly appearing variables (here \( y \) and \( z \)) constant. With this convention, the subscript \( s \) in (5) may be omitted and rewritten as:

\[
\frac{\partial r}{\partial t} = \frac{\partial x}{\partial t} \frac{\partial f}{\partial x} + \frac{\partial y}{\partial t} \frac{\partial f}{\partial y} + \frac{\partial z}{\partial t} \frac{\partial f}{\partial z} \tag{6}
\]

In a similar way, we get:

\[
\frac{\partial r}{\partial s} = \frac{\partial x}{\partial s} \frac{\partial f}{\partial x} + \frac{\partial y}{\partial s} \frac{\partial f}{\partial y} + \frac{\partial z}{\partial s} \frac{\partial f}{\partial z} \tag{7}
\]

Equations (6) and (7) are known as **chain rules for partial differentiation**.

---

### WORKED OUT EXAMPLES

**Example 1:**  
If \( u = x^2 - y^2 \), \( x = 2r - 3s + 4 \), \( y = -r + 8s \), find \( \frac{\partial u}{\partial r} \) and \( \frac{\partial u}{\partial s} \).

**Solution:**  
Here \( u \) is a function of \( x, y \) which are functions of \( s, t \). So by chain rule:

\[
\frac{\partial u}{\partial r} = \frac{\partial u}{\partial x} \frac{\partial x}{\partial r} + \frac{\partial u}{\partial y} \frac{\partial y}{\partial r}
\]

\[
\frac{\partial u}{\partial s} = \frac{\partial u}{\partial x} \frac{\partial x}{\partial s} + \frac{\partial u}{\partial y} \frac{\partial y}{\partial s}
\]

\[
\frac{\partial u}{\partial x} = 2x, \quad \frac{\partial u}{\partial y} = -2y, \quad \frac{\partial x}{\partial r} = 2, \quad \frac{\partial y}{\partial r} = -1, \quad \frac{\partial x}{\partial s} = -3, \quad \frac{\partial y}{\partial s} = 8
\]

\[
\frac{\partial u}{\partial r} = 2x(2) - 2y(-1) = 4x + 2y
\]

\[
\frac{\partial u}{\partial s} = 2x(-3) + (-2y)(8) = -6x - 16y
\]

\[
\frac{\partial u}{\partial r} = 4(2r - 3s + 4) + 2(-r + 8s) = 8r - 12s + 16 - 2r + 16s = 6r + 4s + 16y
\]

\[
\frac{\partial u}{\partial s} = -6(2r - 3s + 4) - 16(-r + 8s) = -12r + 18s - 24 + 16r - 128s = 4r - 110s - 24
\] 

---


Multiply (1) by `x` and (2) by `y` and adding, we get

\[
x\frac{\partial^2 V}{\partial x^2} + y\frac{\partial^2 V}{\partial y^2} = \left( x\frac{\partial^2 V}{\partial x^2} + x\frac{\partial^2 V}{\partial x \partial y} + x\frac{\partial^2 V}{\partial y \partial x} + y\frac{\partial^2 V}{\partial y^2} + y\frac{\partial^2 V}{\partial y \partial x} + y\frac{\partial^2 V}{\partial x \partial y} \right)
\]

Since 

\[
\frac{\partial^2 V}{\partial x \partial y} = \frac{\partial^2 V}{\partial y \partial x}
\]

The R.H.S. gets simplified to

\[
\frac{\partial^2 V}{\partial x^2} + \frac{\partial^2 V}{\partial y^2} = (x+y)\left( \frac{\partial^2 V}{\partial x^2} + \frac{\partial^2 V}{\partial y^2} \right) + x\frac{\partial^2 V}{\partial x \partial y} + y\frac{\partial^2 V}{\partial y \partial x}
\]

### Exercise

1. If \( V = u^2v \) and \( u = e^{x^2 - y^2}, v = \sin(xy^2) \) find \( \frac{\partial V}{\partial x} \) and \( \frac{\partial V}{\partial y} \).

   **Ans.** 

   \[
   \frac{\partial V}{\partial x} = 2u\frac{\partial u}{\partial x} v + u^2\frac{\partial v}{\partial x} = 2x e^{x^2 - y^2}\left[4x \sin(xy^2) + y^2 \cos(xy^2)\right]
   \]

   \[
   \frac{\partial V}{\partial y} = 2u \frac{\partial u}{\partial y}v + u^2 \frac{\partial v}{\partial y} = 2ye^{x^2 - y^2}xy^2 \cos(xy^2) - 2 \sin(xy^2)
   \]

2. Find \( \frac{\partial V}{\partial y} \) if \( V = (x+y)/(x^2 - xy) \) and \( u = \tan(2r - 2\theta), v = \cot(r^2) \).

   **Ans.**

   \[
   -\left(1 + x(1+y)^2(2x + 2y)/(x^2 - 2xy)^2\right)
   \]

3. If 

   \[
   \frac{\sinh x}{\cos y} \text{ where } u = \cosh x \text{ and } v = \sin x
   \]

   find 

   \[
   \frac{\partial u}{\partial x} \text{ and } \frac{\partial v}{\partial y}
   \]

   **Ans.**

   \[
   \left(u \cos x \cos u \sin y + z \sin x y/\cos y \sin x y/\cos x y\right)
   \]

4. Prove that 

   \[
   \frac{\partial u}{\partial x} = \frac{u}{\cos x} \text{ if } u = e^{x^2 - y^2} + \frac{\sin x}{\cos y}
   \]

   **Ans.**

   \[
   \frac{\partial u}{\partial x} = \frac{u}{\cos x} \frac{\partial v}{\partial x}
   \]

5. If \( \cos x = u + v \) and \( u = \sin x, v = \cos x \) find the total derivative of \( w.r.t. x \).

   **Ans.**

   \[
   \frac{du}{dx} = \frac{\sin x \cos x \tan x \cos x}{\cos^2 x}
   \]

6. Prove that 

   \[
   \frac{\partial^2 u}{\partial x \partial y} = \frac{u}{\cos x}
   \]

   if 

   \[
   V = (1 - 2xy + y^2)^{-\frac{3}{2}}
   \]

7. Show that 

   \[
   \left(\frac{\partial^2 u}{\partial x^2}\right)^2 + \left(\frac{\partial^2 u}{\partial y^2}\right)^2 + \left(\frac{\partial^2 u}{\partial z^2}\right)^2 = \left(\frac{\partial^2 u}{\partial t^2}\right)^2
   \]

   when \( u \) is a function of \( x, y, z \) where \( x = r \cos \theta, y = r \sin \theta \).

8. If \( v = f(r, s, t) \) and \( f \) is a function of \( v = \sqrt{z} \) show that \( \frac{\partial v}{\partial z} = 0 \).

9. Change the Laplacian equation in Cartesian coordinates \( \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0 \) into polar coordinates.

   **Hint:** Use the change of variables \( u = r \cos \theta, v = r \sin \theta \) or \( x = x^2 + y^2, z = z^2 \).

   **Ans.**

   \[
   \text{tan}^{-1}(y/x), \text{ calculate } u = u_r, u_\theta, \text{ etc.}
   \]

10. If \( v = f(u, x) \) where \( u = a \cosh x \cos v, v = a \sinh x \sin v \) prove that 

    \[
    \frac{\partial u}{\partial x} + \frac{\partial v}{\partial x} = \frac{1}{2}(\cosh 2x - \cos 2y) \frac{\partial u}{\partial x}
    \]

11. Transform the Laplacian equation 

    \[
    \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0
    \]

    by changing variables from \( x, y \) to \( \theta, \phi \) when \( x = \cos \theta, y = \sin \theta \).

    **Hint:** Use \( r = \ln \sqrt{x^2 + y^2}, \theta = \text{tan}^{-1}(y/x) \).

    **Ans.**

    \[
    e^{-2}\left(\frac{\partial^2 u}{\partial x^2}\right)^2
    \]

12. Transform the Laplacian 

    \[
    \frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} + \frac{\partial^2 u}{\partial z^2}
    \]

    by changing the variables from \( u, v, w \) to \( x, y, z \) when \( x = \cos \theta - \sin \theta, y = \sin \theta \cos \theta \).

    **Hint:** Use chain rule 

    \[
    u = \text{tan}^{-1}(y/x).
    \]

    **Ans.**

    \[
    \frac{\partial^2 u}{\partial x \partial y} = 0
    \]

13. Express \( \nabla f = \left(\frac{\partial f}{\partial x}\right) + \left(\frac{\partial f}{\partial y}\right)\) in plane polar coordinates.

    **Hint:** Use \( x = r \cos \theta, y = r \sin \theta \), use chain rule.

    **Ans.**

    \[
    \nabla f = f_r \cos \theta - f_\theta \sin \theta = \left(\sin \theta \frac{\partial f}{\partial r} + \cos \theta f\right)
    \]

14. If \( x = r \cos \theta, y = r \sin \theta \) prove that

    \[
    \left(\frac{\partial^2 r}{\partial x^2}\right)^2 + \left(\frac{\partial^2 r}{\partial y^2}\right)^2 = \left(\frac{\partial^2 r}{\partial x \partial y}\right)^2
    \]

**Hint:** 

\[
r_{xx} = \frac{1 - r^2}{x^2}, r_{xy} = -r^2, r_{x} = \frac{-r^2}{xy}
\]

15. If \( u = x^2 + 2xy - \ln z \) where 

\[
x^2 + r^2, y = -r^2, z = 2t
\]

find 

\[
\frac{\partial u}{\partial x} \text{ and } \frac{\partial u}{\partial y} 
\]

at \( (1, 2, 1) \).

**Ans.**

\[
\frac{\partial u}{\partial x} = 4x + 2y - \ln z, \quad \text{at } (1, 2, 1): 8 
\]

\[
\frac{\partial u}{\partial y} = 4y + 2r \ln z - \frac{2y}{z}, \quad \text{at } (1, 2, 1): 8r - 4.
\]

### 3.6 DIFFERENTIATION OF AN IMPLICIT FUNCTION

An implicit function of \( x \) and \( y \) is an equation of the form 

\[
f(x, y) = 0
\]

which cannot necessarily be solved for one of the variables say \( x \) in terms of the other variable say \( y \).

For example 

\[
x^2 + y^2 + a^2 = 0 \tag{1}
\]

is an implicit function which cannot be solved for say \( x \) in terms of \( y \) explicitly. If \( (1) \) defines \( y \) as a function of \( x \), the derivative of \( y \) w.r.t. \( x \) can be calculated in terms of \( y \), without solving \( (1) \) explicitly for \( x \) in the form \( y = y(x) \), by differentiating \( (1) \) partially w.r.t. to \( x \) as 

\[
\frac{\partial f}{\partial x} \frac{dx}{dx} + \frac{\partial f}{\partial y} \frac{dy}{dx} = 0 \tag{2}
\]

solving (2) we get 

\[
\frac{dy}{dx} = - \frac{f_x}{f_y} \quad \text{provided } f_y \neq 0 \tag{3}
\]

Higher derivative of an implicit function \( (1) \) can be obtained by differentiating \( (3) \) on both sides, keeping in mind that the arguments on the right of \( (3) \) are \( x \) and \( y \) itself in the function of \( x \) defined by \( (1) \).

Differentiating \( (3) \) w.r.t. \( x \), noting that \( f_x \) and \( f_y \) are composite functions of \( x, y \), we have 

\[
\frac{d^2 y}{dx^2} = \frac{\partial}{\partial x} \left( -\frac{f_x}{f_y} \right) = \frac{f_{xx} + \frac{\partial f_{xy}}{\partial y}}{(f_y)^2} + \frac{f_x \frac{\partial f_{xy}}{\partial y}}{(f_y)^2} + \frac{\partial f_x}{\partial y} \frac{\partial f_y}{\partial y} \frac{\partial f_y}{\partial x} \frac{\partial f_y}{\partial y} \tag{4}
\]

Substituting from \( (3) \) 

\[
\frac{dy}{dx} = - \frac{f_x}{f_y}
\]

in \( (4) \) and rearranging, we get 

\[
\frac{d^2 y}{dx^2} = \left[ \frac{f_{xx}(f_y)^2 - 2f_x f_y f_{xy} + f_x f_{xy}^2}{(f_y)^3} \right] \tag{5}
\]

if \( f_y \neq 0 \).

Thus \( \frac{dy}{dx} \) and \( \frac{d^2 y}{dx^2} \) given by \( (3) \) and \( (5) \) respectively, are expressed in terms of the partial derivatives \( f_x, f_y, f_{xx}, f_{xy}, f_{yy} \).

### Implicit Function of Three Variables

Let \( f(x, y, z) = 0 \) be the equation of an implicit function of three variables \( x, y, z \). Suppose \( y \) and \( z \) are functions of \( x \), then \( f \) is a function of one independent variable \( x \) and \( y, z \) are intermediate variables.

Keeping \( z \) constant, differentiating w.r.t. \( x \), we get 

\[
\frac{\partial f}{\partial x} + \frac{\partial f}{\partial y} \frac{\partial y}{\partial x} = 0 
\]

solving 

\[
\frac{dy}{dx} = - \frac{\frac{\partial f}{\partial x}}{\frac{\partial f}{\partial y}} \quad \text{provided } f_y \neq 0
\]

Similarly differentiating w.r.t. \( x \), holding \( y \) constant 

\[
\frac{\partial f}{\partial x} + \frac{\partial f}{\partial z} \frac{\partial z}{\partial x} = 0 
\]

solving 

\[
\frac{dz}{dx} = - \frac{\frac{\partial f}{\partial x}}{\frac{\partial f}{\partial z}} \quad \text{if } f_z \neq 0
\]

### Worked Out Examples

#### Implicit function of two variables

**Example 1:** Find \( \frac{dy}{dx} \) from the given implicit function \( f \) connecting \( x \) and \( y \):

a. \( f(x, y) = y \sin(x - y) - (x + y) = 0 \)

   \[
   \frac{dy}{dx} = \frac{\sin(x - y) + \text{sin}(x - y)\left[ 1 - 1 \right]}{x \cos(x - y) - (1 - 1)}
   \]

b. \( y^x = x \log y \)

   Taking \( \log f = y \log x - x \log y = 0 \), 

   \[
   \frac{dy}{dx} = \frac{y}{x} - \frac{y \log y}{\log x} = \frac{\log y}{\log x} 
   \]
```

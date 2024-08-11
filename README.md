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

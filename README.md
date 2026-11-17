# GTU Maths 2 analytic function from the real part u(x,y): harmonic check, conjugate v, f(z) and f'(z)

GTU Hero's Maths 2 guide lists analytic functions, Cauchy-Riemann equations and differentiation of complex functions under complex analysis for BE Mathematics 2 (BE02000011, and older 3110015 papers that include this unit). A common ask: given the real part u(x,y), show it is harmonic, find the conjugate v, and write f(z) = u+iv and f'(z). u(x,y) daalo, this page does the Laplace check, integrates the CR equations with exact fractions, and builds f'(z) = u_x(z,0) - i u_y(z,0). Practice expressions are my own, not from a GTU paper. Laplace 0 nahi aaya toh analytic function exist nahi karta.

Live page: https://princeadvant.github.io/gtu-maths-2-analytic-function-from-u/

## Facts used

- u is the real part of an analytic function only if it is harmonic: u_xx + u_yy = 0 (Laplace's equation).
- Cauchy-Riemann: v_x = -u_y and v_y = u_x. Integrate the first, then use the second to find the function of y.
- Then f'(z) = u_x - i u_y, evaluated on y = 0, x = z, and integrate to get f(z) up to an imaginary constant.
- Default: u = x^2 - y^2 gives v = 2xy + c, f(z) = z^2 + i c and f'(z) = 2z. Also try x^3-3*x*y^2 (that is Re(z^3)) or exp(x)*cos(y) (that is Re(e^z)).

## Test

`node test.js` checks the calculations against hand-worked values and prints `All checks passed`.

## Tips

- In the answer book, show u_xx and u_yy before writing v. The harmonic check carries marks.
- The conjugate is unique only up to a real constant c. Write + c (or + i c in f(z)). Forgetting it is a common half-mark cut.
- If the question gives v instead of u, the same idea works with the CR signs swapped.
- This page handles polynomials in x and y, plus e^x cos y and e^x sin y. For other forms, do the CR integration by hand and use this as a check on a similar polynomial sum.

Which Maths 2 topics to practise (matrices, ODEs and complex analysis) and how to spot repeated question types: [GTU Hero](https://gtuhero.com/blogs/gtu-maths-2-papers-pyqs-repeated-sums) (GTU Hero is my project).

### What is B-Splines
* B-splines are defined by a polunomial degree and a sequence of knots(i.e. the number and position of knots).
* Spline is a piecewise-polynomial function constructed using low degree polynomials which are continuously connected with smoothness conditions at joining points and the abscissas of these points are called 'knots'. The order of the spline m resembles the degree p of the used polynomial segments plus one (m = p +1) or the number of polynomials coefficients.( For instance, the cubic splines are constructed by third-degree polynomial and therefore, their order is m = 4).
* The order of spline function determines the smoothness of picecewise-defined curve since the derivatives up to order m-2 of adjacent polynomial segments must fit together at joining points
*  A spline function is determined by the degree of the polynomial "pieces", the polynomial coefficients and a collection of non descending knot values known as a knot vector or a knot sequence
*  Each click created a new area to the line ( line segment). Each click also creates what's called a control point, or points that determine the shape of the curve. That's the gist of a spline. They create smooth curves out of irregular data points.
### what is the challenge for B-splines
* the identification of the number of knots 
* their respective locations in non-uniform space in the most efficient computational cost
### What is B-splines useful
* B-splines are very useful and popular tools for curve estimations in numerous applications.
### Why we need to optimize B-splines
* when the data forms a smooth curve, many existing methods are avacable to solve the knots without any problems
* when the curves contain non-trivial cases(e.x: discontinuous points, cusps points, cusps, truing points
* too large number of knots can result in serious overfitting of the experimental data.
### Which method can be used to optimize the knot sequence
* Gauss-Newton
### How we can optimize B-splines
* Free knot splines
* non-equidistant knot placement for the curve approximation 
### What is global analytic function?
* There is a point $x_0 \in \R$ such that the Taylor series of f at x_0 exists and converges to f on all of \R.
* There is a point x_0 \in \R such that f has a power series at x_0 that converges to f on all of \R.
* For every point x_0 \in \R, the Taylor series of f at x_0 exists and converges to f on all of \R.
* For every point x_0 \in \R, f has a power series at x_0 that converges to f on all of \R.
### What is banded matrix?
* banded matrix is a sparse matrix whose non-zero entries are confined to a diagonal band, 
* comprising the main diagonal and zero or more diagonals on either side.
### Many-body problem
* a general name for a vast category of physical problems pertaining to the properties of microscopic here implies that quantum mechanics has to be used to provide an accurate deseription of the system.
*  Many-body Schrodinger equation-- are the many-body knietic energy and potential energy operates seperately
*  Many-body wavefunction -- Contains the quantum probalility amplitude for every possible configuration of electrons
### Knot sequence
* is a finite or bi-infinite nondecreasing sequence of real numbers without accumulation points
### what is trivial and non-trivial
* the trivial usually refers to a simple technical aspect of some proof or difinition
* the non-trivial is commonly used to indicate that the example or a solutin is not simple, or that a statement or a theorem is not easy to prove.
### How to use neural networks to recognise knots
### Penalised splines(P-Splines
### Basic Splines(B-Splines)
### What is K-fold Cross Validation?
* Cross validation is an example of a resampling method
* The primary use of cross validation is to select the best tuning parameters
### What is Bootstrap?
* Bootstrap is an example of a resampling method
* Its primary use is uncertainty estimation
* If you have a set of n data points(x1,x2,...,xn) then the bootstrap method would take a sample of these of size n 
  whith replacement so some of the data points may be repeated multiple times and others may not get selcted at all
* Measuring the statistic of interest for each of these bootstrapped samples then allows you to determine the variance of that statistic
### The importance of knot positioning
* The positions of the Knots for a spline can have a very large impact on how good a fit it provides to the data points
* A poor selection of the location of knots can lead to splines that are not even competitive with a simple polynomial regression
### How to use genetic algorithm to improve our knot placement
* Evaualting estimator performance
### How to choose the number and locations of the Knots
* one potential place would be the area of high variability for in those regions the polynomial coefficients can change rapidly
* one option is to place more knots in place where we feel the function might vary most rapidly and to place fewer knots where it seems more stable
* in practice it is common to place knots in a uniform fashion
* another option is to try out different numbers of knots and see which produces the best looking curve.
* 

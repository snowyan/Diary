# Optimization Methods
### what is optimization algorithm 
* Optimization algorithm is a procedure which is executed iteratively by comparing various solutions till an optimum or a satisfactory solution is found.
### the tpye of optimization algorithms
* Deterministic Algorithms -- They use specific rules for moving one solution to other. These algorithms are in use to suite some times and have been successfully applied for many engineering design problems.
* Stochastic Algorithms -- The stochastic algorithms are ni nature with probabilistic translation rules. These are gaining popularity due to certain properties which deterministic algorithms do not have.
### Optimal problem formulation:
* A naive optimal design is achieved by comparing a few alternative solutions created by using a priori problem knowledge.
* First step is investigating the method feasibility of each design solution
* Then Estimate of underlying objective of each solution is compared and best solution is adopted
### Design variables
* There are many design parameters in a design problem and which some are highly sensitive to the proper working of the design, and these parameters are called design variables in the parlance of optimization procedures.
### Constraints
* The constraints represent some functional relationships among the design variables and other design parameters satisfying certain physical phenomenon and certain resource limitations.
* There are two types of constriants. One is inequality type constraints and the other is equality type constraints.
* Inequality constraints state that the functional relationships among variables are either greater than, smaller than or equal to a resource value.
* Equality constraints state that functional relationships should exactly match a resource value.
### Objective functions:
* the objective function can be of two types. Either it is to be maximized or it has to be minimized.
### Variable bounds:
* The final task of the formulation procedure is to set the minimum and the maximum bounds on each design variable.
* One way to remedy this situation is to make a guess about the optimal solution and set the minimum and maximum bounds so the optimal solution lies within these two bounds.
### After the above four tasks are completed, the optimization problem can be mathematically written in a special format, known as nonlinear programming(NLP) format.
![Optimal Structure](/optimal_structure.png "Optimal Stucture")
### The Pros and Cons of Greedy
* Easy to implement
* Computationally efficient
### Brute Force Algorithm
* Enumerate all possible combinations of items
* Remove all of the combinations whose total units exceeds the allowed weight
* From the remaining combinations choose any one whose value is the largest
* Implement using search tree
### the search tree's computational complexity
* Time based on number of nodes generated
* Number of levels is number of items to choose from
* Number of nodes at level i is 2^i
* So, if there are n items the number of nodes is O(2^(n+1))
* An obvious optimization: don't explore parts of tree that violate constraint
### Optimal substructure
* a globally optimal solution can be found by combining optimal solutions to local subproblems
### Overlapping subproblems:
* finding an optimal solution involves solving the same problem multiple times
### Summary of Lectures 1-2
* Many problems of practical importance can be formulated as optimization problems
* Greedy algorithms oftern provide adequate(though not necessarily optimal) solutions
* finding an optimal solution is usually exponentially hard
* Bit dynamic programming ofter yields good performance for a subclass of optimization problems -- those with optimal substructure and overlapping subproblems
  Solution always correct
  Fast under the right circumstances


# 7.1. Formal definition

In the more general approach, an optimization problem consists of maximizing or minimizing a real function by systematically choosing input values from within an allowed set and computing the value of the function. More generally, optimization includes finding 'best' values of some objective function given a defined domain (or input), including a variety of different types of objective functions and different types of domains.

An optimization problem can be represented in the following way:

* Given: a function $f : A \rightarrow {R}$ from some set $A$ to the real numbers ${R}$.

* Sought: an element $x_0 \in A$ such that $f(x_0) \leq f(x)$ for all $x \in A$ ('minimization') or such that $f(x_0) \geq f(x)$ for all $x \in A$ ('maximization').

Such a formulation is called an **optimization problem** or a mathematical programming problem (a term not directly related to computer programming, but still in use for example in linear programming). Many real-world and theoretical problems may be modeled in this general framework.

Typically, $A$ is some subset of the Euclidean space ${R}^n$ [^euclidean], often specified by a set of constraints, equalities or inequalities that the members of $A$ have to satisfy. The domain $A$ of $f$ is called the **search space** or the feasible set, while the elements of $A$ are called **candidate solutions** or feasible solutions.

The function $f$ is called, variously, an **objective function**, a loss function or cost function (minimization), a utility function or fitness function (maximization), or, in certain fields, an energy function or energy functional. A feasible solution that minimizes (or maximizes, if that is the goal) the objective function is called an **optimal solution**.

In mathematics, conventional optimization problems are usually stated in terms of minimization.

A **local minimum** $x^*$ is defined as an element for which there exists some $δ \geq 0$ such that:

$\forall x \in A$ where $| x − x^∗ | ≤ δ$, the expression $f(x^*) \leq f(x)$ holds;

That is to say, on some region around $x^*$ all of the function values are greater than or equal to the value at that element. Local maxima are defined similarly.

While a local minimum is at least as good as any nearby elements, a global minimum is at least as good as every feasible element. Generally, unless the objective function is convex in a minimization problem, there may be several local minima.

## Constraints, goals and objectives

Zeleny [^Zeleny] describes the conceptual and technical differences between constraints, goals, and objectives:

* **A constraint** is a fixed requirement which cannot be violated in a given problem formulation. Constraints divide all possible solutions into two groups: feasible and infeasible.
* **A goal** is a fixed requirement which is to be satified as closely as possible in a given problem fomulation.
* **An objective** is a requirement which is to be followed to the greatest extent possible (either by minimization or maximization) given the problem's constraints.


[^euclidean]: Euclidean space, denoted as ${R}^n$, is a mathematical construct that represents a space of $n$ dimensions where the geometry is defined by Euclid's axioms, i.e. a space in which we can measure distances and angles.
[^Zeleny]: Zeleny, M. (1982). Multiple Criteria Decision Making. McGraw-Hill.
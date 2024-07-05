# 7.2. Optimization process

Before the optimization process can be started the optimization problem needs to be formulated. For this a distinction needs to be made between the **controlled variables** (sometimes called the endogenous variables), the **uncontrolled variables** (sometimes called the exogenous variables), **objective(s)** and **constraints**.

By means of an optimization algorithm, the controlled variables are changed and evaluated using the objective and constraints. The uncontrolled variables link controlled variables to the objective(s). This search process ends when the found solution can no longer be improved.

## The XYZ production problem

Consider XYZ Corporation builds two computer models – the Standard and the Deluxe. The Standard has a profit per unit of $300, and the Deluxe has a profit per unit of $500. The two models are produced from three components: the Standard computer tower (60 in stock), the Deluxe computer tower (50 in stock), and a hard drive (120 in stock).

What combination of Standard and Deluxe computer towers will maximize XYZ's profit from the components currently in stock?

For this problem the controlled variables are the number of Standard and Deluxe computer towers. The uncontrolled variables are the profit per unit. The objective is the total profit which needs to be maximized. The constraints are the number of Standard and Deluxe computer towers in stock, and also the number of hard drives in stock.

Because of the simplicity of this optimization problem we are able to solve it graphically.

Figure X: Graphical representation of the XYZ production problem.

The **constraints** define the **solution space** (feasible region) which contains all allowed solutions, in this example the combinations of computer towers produced. The **objective function** and its direction (maximize/minimize) determine what is considered the **optimal solution**.

## Discrete optimization and continuous optimization

In the case of the computer production problem the controlled variables are **discrete** as it is not feasible to manufacture fractions of computers. Discrete controlled variables will negatively impact the time to find an optimal solution. It can sometimes be useful to consider discrete controlled variables as being continuous. The output will then give a rough estimate of the ideal solution after rounding the different variable to the nearest integer value.

Depending on the type of optimization problem it is also possible that the controlled variables are **continuous**. In this case the optimization algorithm is not limited to integer variable values. Having only continuous variables will positively impact the time to find an optimal solution.

A mix of discrete and continuous variables is also not uncommon. In case of linear programming this is called **mixed integer linear programming (MILP)**.

## Constrained and unconstrained optimization

Typical text books on mathematical optimization start with problems that are **unconstrained**. Such simplified problems allow for conveying the concept of mathematical optimization. The figure at the start of this chapter is a typical example of such a simplified problem.

However, in real life applications of optimization techniques, problems are unlikely to be unconstrained. 
The computer production problem was constrained by the amount of computer towers and hard drives in stock.

In engineering it is likely that the optimization problem is **constrained** by laws that are derived from the natural sciences. It is not uncommon that the problem is also constrained in the sense that stakeholders have set limits on different variables. The most common example is a budgetary constraint that cannot be violated but has no relation to the natural sciences, rather is related to the social sciences.

There is a clear distinction between constraints that are derived from the natural sciences and from the social sciences. The former are fixed and cannot be violated (non-negotiable) whereas the latter can still be up for debate (negotiable).

## Linear and non-linear optimization

When both the objective and constraint functions are linear, the optimization problem is considered a **linear optimization problem**. Linear optimization problems are easier to solve than general nonlinear ones.

The first numerical optimization algorithms were developed to solve linear optimization problems, and there are many applications in operations research.

When the objective function is quadratic and the constraints are linear, we have a **quadratic optimization problem**, which is another type of problem for which specialized solution methods exist. 

Functions can be either **uni-modal** or **multi-modal**. Uni-modal functions have a single minimum, whereas multi-modal functions have multiple minima. When we find a minimum without knowledge of whether the function is uni-modal or not, we can only say that it is a **local minimum**; that is, this point is better than any point within a small neighborhood.

Often, we need not be too concerned about the possibility of multiple local minima. From an engineering design point of view, achieving a local optimum that is better than the initial design is already a useful result.

**Convexity** is a concept related to multi-modality. A function is convex if all line segments connecting any two points in the function lie above the function and never intersect it. Convex functions are always uni-modal. Also, all multi-modal functions are non-convex, but not all uni-modal functions are convex.

**Convex optimization** seeks to minimize convex functions over convex sets. Like linear optimization, convex optimization is another subfield of numerical optimization with many applications. When the objective and constraints are convex functions, we can use specialized formulations and algorithms that are much more efficient than general nonlinear algorithms to find the global optimum.

# 5.2. Decision making process

In a design process choice making occurs after generating design alternatives. At that moment the designers have a set of alternative (sub)solutions and alternative combinations of (sub)solutions. All these solutions together form the so-called design space; An imaginary space that contains or envelopes all the potential solutions to the design problem [Dym and Little, 2004] [^Dym].

Which design alternative is the optimum choice; the 'best'? Which of the alternatives will provide the best result when set against the requirements and the preferences of all stakeholders? These assessments are subjective by definition, and are based on the preferences of everyone involved in the design project.

A **decision matrix** is a tool that is typically used by architectural and urban planners for finding the “best” combination. The individual items in a decision matrix represent the scores of an alternative (design solution) on a specific criterion (functionality, effectiveness, style, cost, etc.). Aggregating scores is done my multiplying an alternative’s score on each criterion by the assigned weight attached to that criterion.

## Decision matrix

A decision matrix is mathematically expressed as follows:

$ V(x)=\sum_{i=1}^{n} w_iv_i(x_i) $

Where $V_i(x_i)$ is the **value** or performance of alternative $x$ on the $i$th criterion, $w_i$ is the **importance weight** of the $i$th criterion and $n$ is the **number of different criteria**.

The choice problem can then be “solved” by using a mathematical model (of the rating scale) to calculate the best alternative. The rating scale used in a decision matrix is the foundation of the mathematical representation of the choice problem.

## Example


|       | $A_1$ | $A_2$ | $A_3$ | Weighting |
| ----- | ----- | ----- | ----- | --------- |
| $C_1$ | 100   | 0     | 67    | 0.67      |
| $C_2$ | 28    | 56    | 37    | 0.33      |
| Value | 67    | 37    | 33    |           |

Stevens [^Stevens] proposed a uniqueness-based classification of scales into nominal, ordinal, interval and ration scales:

* **Nominal scales** represent the most unrestricted assignment of numerals. The numerals are used only as labels or type numbers, and words or letters would serve as well.
* **Ordinal scales** arise from rank ordering. A classic example of an ordinal scale is Möhs scale of mineral hardness which characterizes the scratch resistance of various minerals through the ability of a harder material to scratch a softer material.
* **Interval scales** are scales that are unique up to additive and (positive) multiplicative constants, i.e. the uniqueness of the set of all possible scales is characterized by $t=p+q \times s$.
* **Ratio scales** are scales that are unique up to a multiplicative constant, i.e. the uniqueness of the set of all possible scales is characterized by $t=q \times s$.


Ordinal scales do not enable the operations of addition and multiplication, and the concepts of cancellation and trade-off do not apply to them.

To appreciate the practical implications of ignoring differences and ratios, consider the following example: Two competing designs for a new passenger airplane are compared with respect to their range, fuel consumption and the number of passengers they can carry. Suppose that design A is superior to B with respect to range and fuel consumption but is inferior to B with respect to the number of passengers. See the next table.

|            | Design A | Design B |
| ---------- | -------- | -------- |
| Range      | +        | -        |
| Fuel       | +        | -        |
| Passengers | -        | +        |

Since A is better than B twice while B is better than A once, design A will be chosen over B based on ordinal counting procedures. These procedures ignore the question 'by how much is A better than B?' Indeed, these procedures will indicate a preference for A even if B performs slightly less well as A on range and fuel consumption but can carry twice the number of passengers as A. Note that the concept of 'slightly less' is applicable to proper scales but is not applicable to ordinal ones. In our example, because the concepts of difference, slight difference, large difference or twice are inapplicable in the ordinal methodologies, these methodologies lead to an unacceptable 'cancellation' or 'trade-off' of a slight advantage in fuel consumption against a large advantage in the number of passengers.

**Selection** is an important problem in engineering design. By definition, selection means making choices and choice is synonymous to preference since we choose those objects that are preferred. Therefore, the scientific foundation of selection in engineering design (and elsewhere) is the **measurement of preference**.


## Multi Criteria Decision Making (MCDM)

**Multi-Criteria Decision Making** (MCDM) is on of the most well know branches of decision making. According to many authors MCDM is divided into **Multi-Objective Decision Making** (MODM) making and **Multi-Attribute Decision Making** (MADM). MODM studies decision problems in which the decision space is continuous. A typical example is mathematical programming problems with multiple objective functions. On the other hand MADM concentrates on problems with discrete decision spaces. In these problems the set of decision alternatives has been predetermined.

Although MCDM methods may be widely diverse, many of them have certain aspects in common. These are the notions of alternatives and attributes (also often called decision criteria) as described next.

Usually **alternatives** represent the different choices of action available to the decision maker. In this book the alternatives are supposed to be prioritized, i. e. ranked.

Each MCDM problem is associated with multiple attributes. **Attributes** are also referred to as “goals” or “decision criteria”. Attributes represent the different dimensions from which the alternatives can be viewed.

In cases in which the number of criteria is large, criteria may be arranged in a hierarchical manner. That is, some criteria may be major ones. Each major criterion may be associated with several sub-criteria. Similarly, each sub-criterion may be associated with several sub-criteria and so on. Although some MCDM methods may explicitly consider a hierarchical structure in the criteria of a decision problem, most of them assume a single level of criteria (e. g. no hierarchies).

Different criteria may be associated with different units of measure. For instance, in the case of buying a new car, the criteria “cost” and “mileage” may be measured in terms of dollars and thousands of miles, respectively. It is this nature of having to consider different units which makes MCDM problems intrinsically hard to solve.

## Theory of (preference) measurement

Since the only property of relevance in the context of the mathematical foundations of decision theory is preference, decision making is founded on preference measurement. The correctness of a decision analysis methodology is determined by the correctness of the scales used for this preference measurement. The correctness of scales is defined by whether or not the scales generated allow mathematical operations, for further details see Barzilai [^Brazilai].

The purpose of measurement is “to enable the powerful weapon of mathematical analysis to the subject matter of science”. Phrased formally: the purpose of modeling an **empirical system E** by a **mathematical system M** is to enable the application of mathematical operations on the elements of M.

An empirical system E is a set of empirical objects together with operations which characterize the property under measurement. A mathematical model M of the empirical system is a set with operations that reflect the empirical operation in E as well as the order in E when E is ordered. A **scale s** is a mapping of the object in E into the object in M that reflects the structure of E into M.

If the mathematical operations of addition and multiplication are to be enabled, the mathematical system M must be a one-dimensional **affine space** if it is a model of a system with neither an absolute zero or one which is the case for psychological variables.

The one-dimensional affine space is the algebraic formulation of the familiar straight line of elementary (affine) geometry so that for the operations of addition and multiplication to be enabled on models that characterize subjective properties, i.e. preference, the empirical object must correspond to points on a straight line of an affine geometry.

The operation of addition is defined on point differences, which are vectors. Multiplication of a vector by a scalar is defined and the result is a vector. In the one-dimensional case, and only in this case, the ratio of a vector divided by another non-zero vector is a scalar.

The expression $\frac{a−b}{c-d}=k$ where $a$, $b$, $c$, and $d$ are points on an affine straight line and $k$ is a scalar is used in the construction of proper scales for measuring preference. The number of points in the left-hand side of this expression can be reduced from four to three (e.g. if $b = d$) but it cannot be reduced to two.

Adhering to the above theory of measurement a decision maker’s preference needs to be rated by first establishing two reference alternatives: 
1) a **“bottom” reference alternative** which is rated at 0; 
2) a **“top” reference alternative** which is rated at 100. 
Then the other alternatives are rated relative to these reference alternatives on the scale defined.

## Examples

### Single decision maker problems

Consider a decision maker who wants to buy a new laptop and has narrowed the search down to the following 3 alternatives:

* **Laptop A** costing 599 euro, having a 16 inch screen, a 1TB storage capacity and an AMD Ryzen 7 processor.
* **Laptop B** costing 599 euro, having a 15.6 inch screen, a 512GB storage capacity and an AMD Ryzen 5 processor.
* **Laptop C** costing 709 euro, having a 16 inch screen, a 256GB storage capacity and an AMD Ryzen 5 processor.
* **Laptop D** costing 499 euro, having a 16 inch screen, a 512GB storage capacity and an AMD Ryzen 7 processor.

The decision maker scored each laptop and assigned weights to each criterion as shown in the next table. Note that the decision maker used linear interpolation to determine intermediate scores. For instance, with regards to the criterion price, the decision maker rated a laptop with a price halfway the least and most expensive laptops at 50. The decision maker did the same for the criterion storage capacity.

|                  | Weighting | Laptop A | Laptop B | Laptop C | Laptop D |
| ---------------- | --------- | -------- | -------- | -------- | -------- |
| Price            | 0.5       | 50       | 50       | 0        | 100      |
| Screen size      | 0.2       | 100      | 0        | 100      | 100      |
| Storage capacity | 0.15      | 100      | 50       | 0        | 50       |
| Processor speed  | 0.15      | 100      | 0        | 0        | 100      |


Looking at the scores and weights it is expected that laptop D will have the highest overall preference rating and laptop C the lowest. Laptop D scores highest on all but one criterion with a relatively low weight attached to it. Contrary, laptop C scores lowest on all but one criterion with a low weight attached to it. Laptop A is expected to be a close second because it also scores highest on all but one criterion with a relative high weight attached to it. 

Recall that the scores and weights are subjective and will differ for each person. Consider the scores and weights of another person as shown in the next table. Here the decision maker rated laptops with regards to the criterion price differently and also uses a different weight distribution. In this example the decision maker is more lenient with regards to price and rates laptops with a price halfway the extremes at 75. The decision maker also considers it a less important criterion and attaches most weight to the criterion processor speed.

|                  | Weighting | Laptop A | Laptop B | Laptop C | Laptop D |
| ---------------- | --------- | -------- | -------- | -------- | -------- |
| Price            | 0.3       | 75       | 75       | 0        | 100      |
| Screen size      | 0.2       | 100      | 0        | 100      | 100      |
| Storage capacity | 0.4       | 100      | 50       | 0        | 50       |
| Processor speed  | 0.1       | 100      | 0        | 0        | 100      |


Looking at the scores and weights it is expected that laptop A will have the highest overall preference rating and laptop C the lowest. Laptop A scores highest on all but one criterion with a relatively low weight attached to it. Contrary, laptop C scores lowest on all but one criterion with a low weight attached to it. Laptop D is expected to be a close second because it also scores highest on all but one criterion with a relative high weight attached to it. 

### Group decision making problems

Consider that two decision makers will jointly buy one laptop. We use the information gatherered previously to construct a decision table and assume that the first decision maker is only interested in the laptop's price and screen size while the other decision maker is only interested in the storage capacity and processor speed. Assuming both stakeholders have the same decision maker power we can construct the following table:

|                  | Weighting | Criteria          | Weighting | Laptop A | Laptop B | Laptop C | Laptop D |
| ---------------- | --------- | ----------------- | --------- | -------- | -------- | -------- | -------- |
| Decision maker A | 0.5       | Price             | 0.3       | 75       | 75       | 0        | 100      |
|                  |           | Screen size       | 0.2       | 100      | 0        | 100      | 100      |
| Decision maker B | 0.5       | Storage capacity  | 0.4       | 100      | 50       | 0        | 50       |
|                  |           | Processor speed   | 0.1       | 100      | 0        | 0        | 100      |

In this way we can also solve group decision making problems. The amount of weight for each stakeholder now represents their power. Determining the weight distribution needs to be approached with great care.

[^Dym]: Dyme, C. (2013). Engineering design: A Project-Based Introduction, Wiley.

[^Stevens]: Stevens, S. S. (7 June 1946). "On the Theory of Scales of Measurement". Science. 103 (2684): 677–680.

[^Ackoff]: Ackoff, R. L. (1999). Ackoff's best: His classic writings on management. (No Title).

[^Brazilai]: Barzilai, J. (2022). Pure Economics, FriesenPress.


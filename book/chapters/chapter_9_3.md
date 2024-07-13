# 9.3. The Stedelijk Museum Amsterdam case

The main problem to solve: which allocation of functions to the primary location (existing building and extension) and secondary location is feasible and most desirable?

### Specify the design variables

The design variables relate to the floor space allocated to 7 functions on the primary $p_1 \ldots p_7$ and 5 functions on secondary location $s_1 \ldots s_5$. 

### Retrieve decision maker's objectives

The following decision makers are identified along with the objectives they are interested in:

* The municipality interested in the investment (objective $i$) which is allowed to range between 71.2 and 73.4 million euros.
* The museum staff interested in the floor space allocated to functions on the primary and secondary location which are allowed to range between values as shown in the table below.

| Space type    | Variable | Minimal | Ideal  |
| ------------- | -------- | ------- | ------ |
| Exhibitions   | $p_1$    | 7 901   | 10 154 |
| Workshops     | $p_2$    | 1 354   | 1 438  |
|               | $s_1$    | 693     | 714    |
| Education     | $p_3$    | 941     | 1 378  |
|               | $s_2$    | 56      | 84     |
| Depots        | $p_4$    | 525     | 721    |
|               | $s_3$    | 7 423   | 9 960  |
| Installations | $p_5$    | 6 264   | 7 031  |
|               | $s_4$    | 1 207   | 1 648  |
| Public        | $p_6$    | 3 167   | 3 990  |
| Offices       | $p_7$    | 1 624   | 2 230  |
|               | $s_5$    | 168     | 281    |

### Determine the preference functions for each objective

The staff rate the minimal floor space values at 0 and the ideal values at 100. Intermediate values are rated according the the below table.

| Space type    | Variable | Intermediate | Rating |
| ------------- | -------- | ------------ | ------ |
| Exhibitions   | $p_1$    | 9 703        | 20     | 
| Workshops     | $p_2$    | 1 375        | 70     |
|               | $s_1$    | 697          | 80     |
| Education     | $p_3$    | 1 050        | 70     |
|               | $s_2$    | 62           | 80     |
| Depots        | $p_4$    | 652          | 35     |
|               | $s_3$    | 7 930        | 80     |
| Installations | $p_5$    | 6 417        | 80     |
|               | $s_4$    | 1 295        | 80     |
| Public        | $p_6$    | 3 702        | 35     |
| Offices       | $p_7$    | 1 776        | 70     |
|               | $s_5$    | 191          | 80     |

The municipality rates a synthetic alternative costing 73.4 million euros at 0, an alternative costing 71.2 million euros at 100 and an intermediate alternative costing 71.8 million euros at 70.

The resulting preference functions are shown in the figure below.

<div style="text-align: center;">
  <img src="./images/smafunctions.png" alt="Chapter 9" width="70%">
</div>


### To each objective assign decision maker's weights

For this problem the weights are assumed to be equal, i.e. $w_1 \ldots w_{13} = \frac{1}{13}$.

### Determine the design constraints

For this experiment the first design constraint relates the floor space and the investment.

The first constraint ensures that the maximum allowed investment cannot be exceeded:

$$
(2\,580 - 2\,950) 14\,142 + 2\,950 \sum_{i=1}^7 p_i+1\,400\sum_{i=1}^5 s_i \leq 74\,000\,000
$$

The second constraint relates the floor space on the central location to the capacity of the existing building and extension:

$$
\sum_{i=1}^7 p_i \leq 14\,142+24\,007
$$

The third relates the floor space on the secondary location to the capacity of the building on the secondary location:

$$
\sum_{i=1}^5 s_i \leq 13\,000
$$

### Find the optimal design having the highest preference score

Running the optimization yields a **local optimal design configuration** [^1] as shown in the figure below. Note that the municipality has 'only' $1/13$th of the weight and that the museum staff has $12/13$th of the weight. This may be debatable, and it is up to the reader to change the model so that both stakeholders have the same weight attached

<div style="text-align: center;">
  <img src="./images/smaresult.png" alt="Chapter 9" width="70%">
</div>






[^1]: The nature of non-linear optimization is such that, if the problem's feasible set is non-empty, it can only find a so-called local optimum. As a result, it may be that, depending on the start point of the search, your optimization run finds a different optimal solution than presented here. This is drawback of non-linear optimization.
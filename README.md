# SciKit_Learn_Regression

Learnt about optimisation technique of the error function using two alogorithms:

1.Gradient Descent(GD)

2. Huber Regressor/Loss (HL)

Since GD squares the error term while minimising, it also squares the outliers. This disturbs the performance. However a counter 
to this would be using the absolute error as the cost function. This too, proves deleterious as at the origin, when curve passes, slope
can't be calculated as a discontinuity has been produced.

![GDescent](https://user-images.githubusercontent.com/55191934/74587444-47aa4600-5018-11ea-8e0c-f7284df43287.PNG)

Hence, as a sort of middle ground to this, Huber Loss function is implemented wherein at the origin and near it's region,
a quadratic function graph is initiated and just starting from it's tips the straight line originates, thereby curbing the issue of 
discontinuity.

As seen below, the Huber line is a bit laid back, trying to encapsulate mre datapoints, than the MSE.
It also solves the issue of outliers.


![Huber](https://user-images.githubusercontent.com/55191934/74587518-8e4c7000-5019-11ea-9cf0-57954a3e86f2.PNG)


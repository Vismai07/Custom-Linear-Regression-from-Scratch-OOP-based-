# Custom-Linear-Regression-from-Scratch-OOP-based

## Objective 

**Cause & purpose of this project**
This project was built with delibrate goal: to move beyond using pre-built machine 
learning libraries and instead understand how learning systems are constructed from first principles.

In most academic or begineers workflows, linear regression is implemenetd using libraries like scikit-learn, where the internal mechanics are hidden. While this is efficient, it does not develop a deep understanding of:

- How models learn from data
- how errors guide improvement
- How to optimzing algorithim actgually works

## Purpsoe
The purpose of this program is threefold:
1. Cocneptual Clarity:
To clearly understand the relationship between data, mathematical models and optimization. Instead of trating ML as a black box, this project exposes every step in training a model

2. System Design THinking:
To demonstrate how machine leanring system can vbe modularized using ibhject oriented programming. By seprating the model, loss fucntion, and optimizier, we replicate the design principles used in real world ML frameworks

3. Founcation for Advanmced Applications:
Linear regression is not just a basic algorithim it is foundation for complex models such as neural networks, time series forecasting model and quantiitive financeial models. Understanding this.
- Predictive modeling in finance(eg. price prediction, risk estimation)
- Machine learning pipe lines
- Optimization based decicion system 




Linear regression tries to model a relationship
$$
y=f(x) \approx \beta_0 +\beta_1x_1+\beta_2x_2+...+\beta_px_p
$$

$$
x_i: fetaure (inputs)
\beta_i: parameters(weights)
y:output
$$

- Approximating an unkown data-generating process(DGP), using linear parametric model.

## Matrix form 
Instead of writing equation one by one we use linear algebra:
$$
y=X\beta+\epsilon
$$

$$
- X \in \mathbb{R}^{n \times p}: design matrix 
- B \in \mathbb{R}^p
- \epsilon: noise(random error)

$$

- This is canocical lienar model use din ecnometrics, ML, and statistics

## Objective Function
We estiamte $\beta$ by minimizing squared error:
$$
min_\beta ||y-X\beta||^2
$$



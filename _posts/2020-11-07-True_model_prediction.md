---
author:
- Mingyang Liu
title: TRUE MODEL MIGHT NOT BE THE BEST PREDICTIVE MODEL
...
--- 

Hagerty and Srinivasan (1991): “We note that the practice in applied research of concluding that a model with a higher predictive validity is “truer,” is not a valid inference.

Lemma: $$MSE = E[(\tilde y - \hat f(\tilde x))^2|\tilde x]=\sigma^2+Bias^2+Variance$$

Let $$y=x'\beta_0+\epsilon, \beta_0=(\beta_{01}, \beta_{02})$$, and $$\hat{f}$$ be its OLS estimator. 

The "TRUE" model satisfies

bias=$$0$$, Variance=$$\sigma^2\tilde x'(X'X)^{-1}\tilde x$$

Consider a parsimonious model $\hat f^* (x)=\hat \gamma x$. Then it satisfies

Bias'=$$(\tilde x_1\frac{X_1'X_2}{X_1'X_1}-\tilde x_2)\beta_2$$, Variance'=$$\sigma^2\tilde x_1^2(X_1'X_1)^{-1}$$

Let $$X_1'X1=X_2'X_2=1, X_1'X_2=\rho$$, then
1. Variance = $$\sigma^2 \frac{1}{1-\rho^2}(\tilde x_1^2-2 \tilde x_1 \tilde x_2+\tilde x_2^2)$$, Bias = 0
2. Variance'= $$\sigma^2 \tilde x_1^2$$, Bias'=$$(\tilde x_1 \rho-\tilde x_2)\beta_{02}$$
3. When $$\rho\rightarrow 1, \beta_2\rightarrow 0, \sigma^2\rightarrow \infty$$, we have Variance'+Bias'<Variance+Bias




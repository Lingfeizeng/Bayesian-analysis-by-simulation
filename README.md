# Bayesian analysis by simulation

### The difference between Frequentist and Baysian:

Y ~ N(μ,σ2)

**Frequentist**: μ and σ2 are fixed
**Bayesian**: μ and σ2 are random variables

**Bayesian inference**: using Bayes Theroem to estimate the parameters of a probability distribution or statistical model

<img src="bayes.png" alt="Bayes Theorem" width="800" hight="600"/>

### Markov Chain Monte Carlo (MCMC)
**Classical Bayesian inference**: the conjugated prior should be chosen so that the resulting posterior density can be recognised as the density of a known distribution. 

**MCMC**: to approximate the posterior distribution of a parameter of interest by random sampling in a probabilistic space.


<img src="mcmc.png" alt="MCMC"/>

### Metropolis-Hastings sampling



**Example**
To simulate the distribution:

yi | μ ~ N(μ,1)

μ ~ t (0, 1, 1)

<img src="Metropolis-Hastings.png" alt="MCMC"/>




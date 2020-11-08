# Bayesian analysis by simulation

## Bayesian inference

Using Bayes Theroem to estimate the parameters of a probability distribution or statistical model


### Bayes Theroem 

<img src="bayes.png" alt="Bayes Theorem" height="500"/>


### The difference between Frequentist and Baysian


Y ~ N(μ,σ2)


**Frequentist**: μ and σ2 are fixed

**Bayesian**: μ and σ2 are random variables



## Markov Chain Monte Carlo (MCMC)


**Classical Bayesian inference**

The conjugated prior should be chosen so that the resulting posterior density can be recognised as the density of a known distribution. 


**MCMC**

To approximate the posterior distribution of a parameter of interest by random sampling in a probabilistic space.


<img src="mcmc.png" alt="MCMC"/>

### Metropolis-Hastings sampling

**Metropolis-Hastings sampling algorithm**

<img src="Metropolis-Hastings.png" alt="MCMC"/>


**Example**


In order to produce samples from the distribution:

yi | μ ~ N(μ,1)

μ ~ t (0, 1, 1)

After some transformation, We will have the target distribition p is propotional to g:

<img src="distribution.png" alt="dist" height="80"/>

where the left side is the target distribution p and the right side is g. We can use Metropolis-Hastings sampling. The following code example used the popular simulation package JAGS (available both in R and Python)

### Code example 

#### Specify the model

<img src="specify_model.png" height="180"/>

#### Set up the model

<img src="set_up_model.png" height="240"/>

#### Run and post processing

<img src="run_model.png" height="120"/>
<img src="post_processing.png" height="400"/>
<img src="post_processing2.png" height="500"/>
















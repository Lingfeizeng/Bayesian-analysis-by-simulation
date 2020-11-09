# Bayesian analysis by simulation

## Bayesian inference

Using Bayes Theroem to estimate the parameters of a probability distribution or statistical model


### Bayes Theroem 

<img src="bayes.png" alt="Bayes Theorem" height="500"/>

Evidence (normalization factor):

<img src="evidence.png" height="80"/>


### The difference between Frequentist and Baysian


Y ~ N(μ,σ2)


**Frequentist**: μ and σ2 are fixed

**Bayesian**: μ and σ2 are random variables



## Markov Chain Monte Carlo (MCMC)


**Classical Bayesian inference**

The conjugated prior should be chosen so that the resulting posterior density can be recognised as the density of a known distribution. 

<img src="prior.png" height="100"/>


**MCMC**

To approximate the posterior distribution of a parameter of interest by random sampling in a probabilistic space. The “Monte Carlo” part is due to the sampling purpose and the “Markov Chain” part describes the way we obtain these samples.


<img src="mcmc.png" alt="MCMC"/>

### Metropolis-Hastings sampling

**Metropolis-Hastings sampling algorithm**

<img src="Metropolis-Hastings.png" />


**Example**


In order to produce samples from the distribution:

yi | μ ~ N(μ,1)

μ ~ t (0, 1, 1)

After some transformation, We will have the target distribition p is propotional to g:

<img src="distribution.png" alt="dist" height="80"/>

where the left side is the target distribution p and the right side is g. We can use Metropolis-Hastings sampling. The following code example used the popular simulation package JAGS (available both in R and Python)

**Code example** 

#### Specify the model

<img src="specify_model.png" height="180"/>

#### Set up the model

<img src="set_up_model.png" height="240"/>

#### Run and post processing

<img src="run_model.png" height="120"/>
<img src="post_processing.png" height="400"/>
<img src="post_processing2.png" height="500"/>

### Gibbs sampling

Gibbs sampling is a method of sampling with multiple parameters. The idea is that we can update multiple parameters by sampling just one parameter at a time, cycling through all parameters and repeating. To perform the update for one particular parameter, we substitute in the current values of all other parameters.

**Gibbs sampling algorithm**

<img src="gibbs.png" />




### MCMC for linear regression

<img src="lr1.png" height="40"/>
<img src="lr2.png" height="100"/>

**Code example**

<img src="lr3.png" height="600"/>
<img src="lr4.png" height="400"/>


### Application

**Latent Dirichlet Allocation (LDA)**

w: the vector of words in the corpus;

z: the vector of topics associated to these words;

We want to infer z based on the observed w in a Bayesian way:

<img src="lda.png" height="60"/>

Reference paper: https://www.jmlr.org/papers/volume3/blei03a/blei03a.pdf

















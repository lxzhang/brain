# Probability Brief Intro

Tags: Probability

> [戳我的作业部落-本文][this]
>
> [戳我的作业部落-文档目录](https://github.com/district10/brain/tree/master/_data/zybuluo)

---

[TOC]

Probability theory is the branch of mathematics concerned with probability,
the analysis of random phenomena. The central objects of probability theory 
are random variables, stochastic processes, and events: mathematical abstractions 
of non-deterministic events or measured quantities that may either be single 
occurrences or evolve over time in an apparently random fashion. 
If an individual coin toss or the roll of dice is considered to be a random event,
 then if repeated many times the sequence of random events will exhibit certain
 patterns, which can be studied and predicted. 
 Two representative mathematical results describing such patterns are 
 **the law of large numbers** and **the central limit theorem**.
 
As a mathematical foundation for statistics, probability theory is essential 
to many human activities that involve quantitative analysis of large sets of data.
Methods of probability theory also apply to descriptions of complex systems 
given only partial knowledge of their state, as in statistical mechanics. 
A great discovery of twentieth century physics was the probabilistic nature 
of physical phenomena at atomic scales, described in quantum mechanics.




## **Probability distribution**

### Terminology

* **Probability mass**, [Probability mass function][pmf], **`p.m.f.`**: for discrete random variables.

![][pic01]

* **Categorical distribution**: for discrete random variables with a finite set of values.
* **Probability density**, [Probability density function][pdf], **`p.d.f.`**: most often reserved for continuous random variables.

![][pic02]

* **Probability distribution function**: continuous or discrete, non-cumulative or cumulative.
* **Probability distribution**: sometimes the same as probability distribution function, but usually refers to the more complete assignment of probabilities to all measurable subsets of outcomes, not just to specific outcomes or ranges of outcomes.

**Basic Terms**

* [Mode][mode]: for a discrete random variable, the value with highest probability 
(the location at which the probability mass function has its peak); 
for a continuous random variable, the location at which 
the probability density function has its peak.
* [Support][support]: the smallest closed set whose complement has probability zero.
* [Head][head]: the range of values where the pmf or pdf is relatively high.
* [Tail][tail]: the complement of the head within the support; 
the large set of values where the pmf or pdf is relatively low.
* [Expected value][expected-value] or mean: the weighted average of the
 possible values, using their probabilities as their weights; 
or the continuous analog thereof.
* [Median][median]: the value such that the set of values less than the median 
has a probability of one-half.
* [Variance][variance]: the second moment of the pmf or pdf about the mean; 
an important measure of the dispersion of the distribution.
* [Standard deviation][standard-deviation]: the square root of the variance, 
and hence another measure of dispersion.
* Symmetry: a property of some distributions in which the portion of the distribution 
to the left of a specific value is a mirror image of the portion to its right.
* [Skewness][skewness]: a measure of the extent to which a pmf or pdf "leans" 
to one side of its mean.


### **Cumulative distribution function**

Because a probability distribution Pr on the real line is determined by
the probability of a scalar random variable X being in a half-open interval (-∞, x], 
the probability distribution is completely characterized by 
its cumulative distribution function:
$$F(x) = \Pr \left[ X \le x \right] \qquad \text{ for all } x \in \mathbb{R}.$$

Cumulative distribution function for the normal distribution:

![][pic03]


### **Discrete probability distribution**

A discrete probability distribution shall be understood as a 
probability distribution characterized by a probability mass function. 
Thus, the distribution of a random variable $X$ is discrete, 
and $X$ is then called a discrete random variable, if

$$\sum_u \Pr(X=u) = 1$$

as u runs through the set of all possible values of X. It follows that 
such a random variable can assume only a finite or countably infinite number of values. 
For the number of potential values to be countably infinite 
even though their probabilities sum to 1 requires that the probabilities 
decline to zero fast enough: for example, if 
$\Pr(X=n) = \tfrac{1}{2^n} for n = 1, 2, ...$, 
we have the sum of probabilities 1/2 + 1/4 + 1/8 + ... = 1.

Among the most well-known discrete probability distributions 
that are used for statistical modeling are 
**the Poisson distribution**, 
**the Bernoulli distribution**, 
**the binomial distribution**, 
**the geometric distribution**, and 
**the negative binomial distribution**. 
In addition, **the discrete uniform distribution** is commonly used in computer programs 
that make equal-probability random selections between a number of choices.

* pmf of a discrete probability distribution. 
The probabilities of the singletons {1}, {3}, and {7} are respectively 0.2, 0.5, 0.3. 
A set not containing any of these points has probability zero.

![][pic04]

* cdf of a discrete probability distribution

![][cdf-discrete]



### **Probability space**

In probability theory, a probability space or a probability triple is 
a mathematical construct that models a real-world process (or "experiment") 
consisting of states that occur randomly. 
A probability space is constructed with a specific kind of situation or experiment in mind. 
One proposes that each time a situation of that kind arises, 
the set of possible outcomes is the same and the probabilities are also the same.

A probability space consists of three parts:

1. A sample space, Ω, which is the set of all possible outcomes.
(注意 Outcome 和 $\omega$(omega))
2. A set of events $\scriptstyle \mathcal{F}$, 
where each event is a set containing zero or more outcomes.
3. The assignment of probabilities to the events; 
that is, a function P from events to probabilities.



### **Measure theoretic formulation**

A measurable function $X \colon A \to B$  between 
a probability space $(A, \mathcal A, P)$ and 
a measurable space $(B, \mathcal B)$  is called 
a discrete random variable 
provided its image is a countable set and the pre-image of singleton sets are measurable, 
i.e., $X^{-1}(b) \in \mathcal A for all b \in B$. 
The latter requirement induces a probability mass function 
$f_X \colon X(A) \to \mathbb R$ via  $f_X(b):=P(X^{-1}(b))$.
Since the pre-images of disjoint sets are disjoint

$$
\sum_{b \in X(A)} f_X(b) = 
\sum_{b \in X(A)} P(X^{-1} (b)) = 
P \left( \bigcup_{b \in X(A)} X^{-1}(b) \right) = 
P(A)=1.
$$

This recovers the definition given above.






---

**See also**

*


**Refs**

* http://en.wikipedia.org/wiki/Probability
* http://en.wikipedia.org/wiki/Probability_space
* http://en.wikipedia.org/wiki/Probability_theory
* http://en.wikipedia.org/wiki/Probability_distribution
* 


[this]: url






[pmf]: http://en.wikipedia.org/wiki/Probability_mass_function
[pdf]: http://en.wikipedia.org/wiki/Probability_density_function
[mode]: http://en.wikipedia.org/wiki/Mode_(statistics)
[support]: http://en.wikipedia.org/wiki/Support_(mathematics)
[head]: http://en.wikipedia.org/wiki/Heavy-tailed_distribution
[tail]: http://en.wikipedia.org/wiki/Heavy-tailed_distribution
[expected-value]: http://en.wikipedia.org/wiki/Expected_value
[median]: http://en.wikipedia.org/wiki/Median
[variance]: http://en.wikipedia.org/wiki/Variance
[standard-deviation]: http://en.wikipedia.org/wiki/Standard_deviation
[skewness]: http://en.wikipedia.org/wiki/Skewness




[pic01]: /_img/2014/pmf.png
[pic02]: /_img/2014/pdf.png
[pic03]: /_img/2014/cumulative-distribution-func-for-normal-distribution.png
[pic04]: /_img/2014/pmf-of-discret-probability-distribution.png
[cdf-discrete]: /_img/2014/cdf-of-discrete-probability-distribution.png
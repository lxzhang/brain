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

![](/_img/2014/pmf.png)

* **Categorical distribution**: for discrete random variables with a finite set of values.
* **Probability density**, [Probability density function][pdf], **`p.d.f.`**: most often reserved for continuous random variables.

![](/_img/2014/pdf.png)

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
![](/_img/2014/cumulative-distribution-func-for-normal-distribution.png)


### **Discrete probability distribution**

A discrete probability distribution shall be understood as a 
probability distribution characterized by a probability mass function. 
Thus, the distribution of a random variable $X$ is discrete, 
and $X$ is then called a discrete random variable, if

$$\sum_u \Pr(X=u) = 1$$

The probability mass function of a discrete probability distribution. 
The probabilities of the singletons {1}, {3}, and {7} are respectively 0.2, 0.5, 0.3. 
A set not containing any of these points has probability zero.
![](/_img/2014/pmf-of-discret-probability-distribution.png)











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

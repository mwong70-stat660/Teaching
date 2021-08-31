Two-Sample Difference
========================================================
author: Moria Wong
date: Aug 6, 2021
autosize: true
transition: rotate

Learning Objectives (LOs)
========================================================

- Distinguish between independent and paired samples.
- Perform a hypothesis test for the difference between two means using the P-value method.

Independent and paired samples
========================================================
![](placebo.gif)

Independent and paired samples
========================================================

A drug company has developed a new drug that is designed to reduce high blood pressure. The researchers wish to design a study to compare the effectiveness of the new drug to that of the old drug. Here are two ways in which the study can be designed.

How can we tell whether a new drug reduces blood pressure better than an old one?

Independent and paired samples
========================================================
#### Design 1: Independent Samples
Two samples of individuals are chosen. One sample is given the old drug and the other sample is given the new drug. After several months, blood pressures of the members of both samples are measured. We compare the blood pressures in the first sample to the blood pressures in the second sample to determine which drug is more effective.

_Independent samples_ mean that the observations in one sample do not influence the observations in the other.


Independent and paired samples
========================================================
#### Design 2: Paired Samples
A single group of individuals is chosen. They are given the old drug for a month, then their blood pressures are measured. They then switch to the new drug for a month, after which their blood pressures are measured again. This produces two samples of measurements, the first one from the old drug and the second one from the new drug. We compare the blood pressures in the first sample to the blood pressures in the second sample to determine which drug is more effective.

_Paired samples_ mean that each observation in one sample can be paired with an observation in the second.

Check your understanding
========================================================
- A sample of students is enrolled in an online statistics class, and another sample is enrolled in a traditional statistics class. At the end of the semester, the students are given a test. The scores from each sample are compared to determine which class was more effective. Are these samples independent or paired?


Learning Objective II
========================================================
- Perform a Hypothesis Test for the Difference Between Two Means Using the P-Value Method


*_Notations:_*

$\mu_1$ and $\mu_2$ are the population means.

$\bar{x}_1$ and $\bar{x}_2$ are the sample means.

$s_1$ and $s_2$ are the sample standard deviations.

$n_1$ and $n_2$ are the sample sizes.



The null and alternate hypotheses
========================================================
The issue is whether the population means $\mu_1$ and $\mu_2$ are equal. The null hypothesis says that the population means are equal:

$H_0: \mu_1 = \mu_2$



There are three possibilities for the alternate hypothesis.

$H_1: \mu_1 < \mu_2$

$H_1: \mu_1 > \mu_2$

$H_1: \mu_1 \ne \mu_2$


The test statistic
========================================================
The test statistic is based on the difference between the two sample means $\bar{x_1} - \bar{x_2}$. The mean of $\bar{x_1} - \bar{x_2}$ is $\mu_1 - \mu_2$.

The sample means $\bar{x}_1$ and $\bar{x}_2$ have variances $\frac{\sigma^2_1}{n_1}$ and $\frac{\sigma^2_2}{n_2}$ respectively.

The population means $\mu_1$ and $\mu_2$ have variances $\sigma^2_1$ and $\sigma^2_2$.

When samples are independent, the variance of the difference $\bar{x_1} - \bar{x_2}$ is the _sum of the variances_, so
 
Variance of $\bar{x_1} - \bar{x_2} = \frac{\sigma^2_1}{n_1} + \frac{\sigma^2_2}{n_2}$


The test statistic
========================================================
The standard error of $\bar{x_1} - \bar{x_2}$ is the square root of the variance. We don't know the values of $\sigma^2_1$ and $\sigma^2_2$, so we approximate them with the sample variances $s^2_1$ and $s^2_2$.

Standard error of $\bar{x_1} - \bar{x_2} = \sqrt{\frac{s^2_1}{n_1} + \frac{s^2_2}{n_2}}$

Test Statistic is

$t=\frac{(\bar{x_1}-\bar{x_2})-(\mu_1 - \mu_2)}{\sqrt{\frac{s^2_1}{n_1}+\frac{s^2_2}{n_2}}}$


Degrees of freedom
========================================================
Under the assumption that $H_0$ is true, the test statistic has approximately a Student’s t distribution.
We need to determine the number of degrees of freedom. There are two ways to do this: a simple method that is easier when computing by hand, and a more complicated method that is used by technology. The simple method is:

Degrees of freedom = Smaller of $(n_1-1)$ and $(n_2-1)$


Assumptions
========================================================
Performing a hypothesis test requires certain assumptions. Assumptions for Performing a Hypothesis Test for the Difference Between Two Means with Independent Samples.

(1) We have simple random samples from two populations.

(2) The samples are independent of one another.

(3) Each sample size is large (n > 30), or its population is approximately normal.

Check to be sure the assumptions are satisfied. If they are, then proceed with the following steps.


Steps for P-Value Method
========================================================
*Step 1:* State the null and alternate hypotheses. 

* The null hypothesis specifies that the population means are equal:
$$H_0: \mu_1 = \mu_2 $$

* The alternative hypothesis will be:
$$ \mu_1 < \mu_2 \text{ or } \mu_1 > \mu_2  \text{ or } \mu_1 \ne \mu_2 $$

*Step 2:* If making a decision, choose a significance level $\alpha$.

*Step 3:* Compute the test statistic

*Step 4:* Compute the P-value. The P-value is an area under the Student’s t curve.

*Step 5:* Interpret the P-value. If making a decision, reject H0 if the P-value is less than or equal
to the significance level $\alpha$.

*Step 6:* State a conclusion.


Take Aways
========================================================
- Two samples are independent if the observations in one sample do not influence the observations in the other.
- Two samples are paired if each observation in one sample can be paired with an observation in the other. Typically the samples consist of pairs of measurements on the same individual, or on pairs of individuals who are related, such as husbands and wives or brothers and sisters.


Next Topics
========================================================
* Exercise problems for p-value method
* Hypothesis test using critical value method
* Construct confidence intervals for the difference between two means.


Reference List
========================================================
* Navidi, W., & Monk, B. (2019). Elementary Statistics (3rd ed., $\S$ 9.1). McGraw Hill.

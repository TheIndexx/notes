---
title: "Logistic Regression"
tags:
- Neural-Networks
- Deep-Learning
enableToc: false # do not show a table of contents on this page
---
#### Text description
An algorithm for [Binary classification](ai/Binary%20classification.md) in [Supervised Learning](ai/Supervised%20Learning.md). In statistics terms, it estimates the probability of an event happening or not, like if you vote or didn't vote, given a dataset. There are only 2 possible outcomes, and the predicted Y value only lies between 0 and 1.

#### Math description
Given x (features), want $\hat{y} = P(y=1|x)$

Parameters: $w \in \mathbb{R}^{n_x}$, $b \in \mathbb{R}$

Output: $\hat{y} = \sigma(w^Tx + b)$

A $\sigma$, or sigmoid function converts whatever number the $(w^Tx + b)$ is to a probability that y = 1, or a range of numbers from 0 to 1. You can look it up if you're interested but I couldn't care less right now.
![](hub/ai/imgs/sigmoidexplanation.png)

Thus, we want to find optimal values of $w$ and $b$ to get $\hat{y}$ to be as accurate as possible, and we can measure this using a [Cost Function](ai/Cost%20Function.md). One method of training the $w$ parameter is known as [Gradient Descent](ai/Gradient%20Descent.md).

---
layout: post
title:  "Performance on top-N recommendations"
date:   2019-09-01 11:00:00 -0400
categories: week3
week: "3"
---

**Paper:** Cremonesi, P., Koren, Y., & Turrin, R. (2010, September). Performance of recommender algorithms on top-n recommendation tasks. In Proceedings of the fourth ACM conference on Recommender systems (pp. 39-46). ACM.

The paper criticizes the typical way of evaluating recommender systems (in 2010), namely the use of error metrics (such as RMSE or MAE), by arguing that accuracy metrics (such as precision or recall) capture better the essence of a top-N recommendation task. Specifically, the authors make a comparison of recommendation methods on accuracy metrics, and they show that methods that perform well on error metrics, does not necessarily perform well on accuracy metrics.
To this end, they compare the performance of some baseline algorithms, some algorithms that performed well on error metrics, and some modified methods to focus on accuracy metrics.
They show that the latter ones perform better.

Also, they present a method to prepare a test set and to calculate the metrics, avoiding biases on the evaluation.
Nonetheless, there are two aspects of their proposal that I don't agree with.
First, I don't like the way they calculate the precision/recall by selecting 1000 non-relevant items and 1 relevant.
They say that this would underestimate the calculated value with respect to the true recall and precision, but they don't explain further why they chose to do it this way. Why should it work with just one relevant item? Does this capture the actual metric?
Second, they stayed on classification-based metrics, precision and recall, and left out ranking-based metrics, such as mean average precision or nDCG. I think ranking metrics can capture even better the user satisfaction when seeing the recommendations provided.


On the other hand, I like that they test the algorithms on the long-tail separately, which answers the question, how would the model perform on not-so-popular items?
This provides an implicit way to test the models on characteristics like novelty and serendipity, and you can easily detect methods that are only good because they recommend the _easy_ items, the most popular ones.


As a conclusion, I think is interesting that they propose a shift from error-based metrics to accuracy-based metrics. The 2010-state-of-the-art was dominated by error metrics, and the best methods shown do not perform well on those, but they do perform well on accuracy metrics. Even more, these kind of metric are more suitable for the task, by providing a closer proxy to user satisfaction (yet not close enough).

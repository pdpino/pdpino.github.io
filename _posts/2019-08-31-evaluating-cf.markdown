---
layout: post
title:  "Evaluating CF"
date:   2019-08-31 14:00:00 -0400
categories: week3
week: "3"
---

**Paper:** Herlocker, J. L., Konstan, J. A., Terveen, L. G., & Riedl, J. T. (2004). Evaluating collaborative filtering recommender systems. ACM Transactions on Information Systems (TOIS), 22(1), 5-53.

The paper presents different aspects to decide how to evaluate a recommender system.
Namely, they categorize three important aspects: the possible user's tasks, the types of dataset characteristics and the types of metrics.
Finally, they discuss other evaluation topics that are not covered by the usual metrics, such as coverage, novelty, and more.


I find interesting how they are implying a framework to design recommender systems.
First, you should determine the user's task.
From the categories they present, the first two are rather obvious, but the rest of them not so much, at least for me.
For instance, the task of _recommending a sequence_ may be very different to the more common _find good items_.
Also, I think the task _find a credible recommender_ is more spreaded now, many methods try to address the explainability aspect, not only on recommendation, but in other ML tasks.

Second, you should characterize your data, by determining the implicit or explicit content, the benefit/cost of a good recommendation, the sampling distribution of the data, and more.
Here, I think is interesting that they talked about _implicit feedback_ without actually saying it, which (I think) wasn't popular at the time.
Though at first they state _"[...] if users don't rate items, the CF recommender systems can't provide recommendations"_, later they discuss _implicit ratings_, which could be items purchases, viewed items, or other things.
Thus, they were talking about _implicit feedback_, before the term was more widely adopted.

Third, and based on the previous analysis, you should define the metrics and aspects to evaluate your system. Here they present three main categories, error, classification and ranking measures.
On the one hand, I think that by now (as opposed to 2004), most of the online systems present the recommendations as a list, independent of the kind of UI used, so the ranking metrics are more suitable.
Nevertheless, you should always consider the specific task and data available, and the classification or error metrics can always be valuable.
On the other hand, the "other things" to evaluate have also become important, such as novelty, user evaluation and explainability, though the latter is not mentioned here as an evaluation aspect.

Finally, the last step in the framework would be designing the solution, testing it, and if necessary, reviewing or iterating through the mentioned steps to improve the results.

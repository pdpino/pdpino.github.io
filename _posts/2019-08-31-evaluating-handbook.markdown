---
layout: post
title:  "Handbook: Evaluation of Recommender Systems"
date:   2019-08-31 14:00:00 -0400
categories: week3
week: "3"
---

**Paper:** Guy, S., & Gunawardana, A.. (2011) “Evaluating recommendation systems.” In Recommender systems handbook, pp. 257-297. Springer US, 2011.

This book chapter presents main aspects of evaluating a recommender system.
Specifically, they present the _how_ you evaluate, the type of study you can use; and the _what_ you evaluate, presented as the the properties that you can measure (or at least try to measure).

They present 3 types of evaluation methods: (1) offline experiments, (2) user studies and (3) online evaluations.
Better than just choosing one, I think is interesting how the three of them are complementary.
I usually thought only of the offline part, by using a dataset, testing different methods with different metrics.
But in a real-life application, it is more appropriate to apply multiple methods, when possible.
For instance, I've heard that sometimes Instagram or Facebook deploy different recommendation algorithms to different users in their platforms, which is an online evaluation of their system.
Nonetheless, is important to keep the order of the evaluations presented, because the risk and costs of them increase. The first is cheaper and provides good candidates; the second delivers insights on the actual user experience; and the third is the ultimate real-life test.

On the other hand, they present about 14 properties to evaluate, which I think it can be a bit overwhelming. Even more, the list could be larger, since they didn't mention some properties that are becoming more popular lately, such as fairness or explainability.
It is practically impossible to perform well on all of them, and measuring them all may take an huge amount of time.
On a real-life application, you should focus on the ones that matter the most for your specific use case, or at least start prioritizing those.

As a conclusion of this paper, you can evaluate performance from many aspects and in many ways, and it is important to decide the best way to do it based on the specific problem or application.

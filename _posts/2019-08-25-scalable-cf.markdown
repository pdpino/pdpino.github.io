---
layout: post
title:  "Scalable CF"
date:   2019-08-25 19:00:00 -0400
categories: week2
week: "2"
---

**Paper:** Takács, G., Pilászy, I., Németh, B., & Tikk, D. (2009). Scalable collaborative filtering approaches for large recommender systems.
{: .paper-name}


The paper presents many variants of the MF model, and compare them with the state-of-the-art implementations on multiple datasets, including the Netflix Prize (very popular at the time).
They present different learning techniques, subsampling techniques, order of the samples when training, and corrections.
Moreover, they argue that the approaches presented are scalable, which is an important requirement of real-life recommender systems.
With these modifications, they show achieve better results, keeping the scalability of th model.
They are even able to explain some recommendations, which, by that time, I think it wasn't a common problem.

The main conclusion to take from the paper, is that the basic algorithms that we are studying are only a baseline. From there you can, and probably should, implement variants to improve performance, scalability, and/or explainability, depending on the specific application.

The authors were very thorough on their analysis, trying to test and explain every aspect of the approaches presented.
Although, I think they could have tried to test more aspects of the recommendation results, than only using RMSE as metric.
For instance, on each approach, which items are getting better or worse results (in terms of RMSE)? and which users?
I think these kind of questions are important to address when using these models as a real-life recommender system.

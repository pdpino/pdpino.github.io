---
layout: post
title:  "Content based RecSys"
date:   2019-09-07 13:00:00 -0400
categories: week4
week: "4"
---

**Paper:** Pazzani, M. J., & Billsus, D. (2007). Content-based recommendation systems. In The adaptive web (pp. 325-341). Springer Berlin Heidelberg. Xu, W., Liu, X., & Gong, Y. (2003). Document clustering based on non-negative matrix factorization. In Proceedings of the 26th annual international ACM SIGIR conference on Research and development in informaion retrieval (pp. 267-273). ACM.
{: .paper-name}


This book chapter presents some aspects of content-based recommendation systems.
They discuss item representation, for instance, how difficult it is to represent free text or non-structured data; they enumerate several algorithms, normally used in classification tasks; and they briefly discussed on the user profile generation, differentiating between information manually entered, using explicit feedback (e.g. ratings), and using implicit feedback.

Though they talked about multiple important topics, I didn't like the narrative and the way they present the explanation.
I missed an overview or big picture of the problem, rather than specific details on different things. The following figure (or a similar one) would have been appropriate, which was shown during a class.

![Content based scheme](/assets/content-based-scheme.png)

They focused on specific algorithms, and they did mentioned trends in the area and some limitations, but they didn't explain it in the context of the different steps and components of a content-based recommender system.
I think that by just reading this paper, you don't get an idea of how to start designing a content-based recommender system. I acknowledge that a person wanting to design such a system would have to read more than one book chapter, but I expected more of an overview on the topic.

Also, opposed to collaborative filtering, the content-based methods are much more specific to the domain.
I expected more emphasis on this fact, and the decisions a researcher has to make when designing such systems, when dealing with images, text or other data.
(Although, by 2007, there may not have been as much development as now in those areas).
One good example that actually was discussed on the paper, is the challenge that free text presents when trying to represent item characteristics.

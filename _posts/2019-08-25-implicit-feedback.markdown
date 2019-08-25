---
layout: post
title:  "CF for Implicit Feedback"
date:   2019-08-25 19:00:00 -0400
categories: week2
---

**Paper:** Hu, Y., Koren, Y., & Volinsky, C. (2008, December). Collaborative filtering for implicit feedback datasets.

The paper presents an explanation of an implicit feedback model, by adapting ideas from matrix factorization with explicit feedback.
They explain very well the differences in the data, assumptions, model, etc.
There are some important differences with explicit feedback, specifically, they enumerate four essential characteristic that makes it different than explicit feedback.
I think the most important difference is the following: the information you get from the user does not mean he/she liked the item, it only means they interacted with the item.
Collaborative Filtering methods need to know, at some degree, the preference of the users, to be able to decide what to recommend.
So, if you only know the interaction with an item, you have to translate this interaction as you think is best, and there is more than one solution for this.

Their solution is rather simple, but it works well. Given the interaction `r_{ui}`, that indicates watch times, they generate the values `c_{ui}` representing confidence, and `p_{ui}` with the preference (0 or 1).
They show other two variants that they could have used, but this is the one with best results.
Moreover, they also come up with a way to explain the recommendation, which makes the model even more powerful.

Is interesting that the system they used is a bit outdated by now, a TV shows system.
More modern systems, such as netflix, have more options to personalize content and to receive user feedback. For instance, they can record user clicks, searches, differentiate multiple users with the same account, and more.
I think that in such a case, they could estimate better some negative feedback, which was a hard task the TV show system. Some ideas:

+ if a user watches an item until less than half, and then stops watching it, is negative feedback
+ if a user gets an item recommended multiple times, and he/she does not watch it, is negative feedback

In any case, the current more resourceful systems can definitely devise ideas to enrich the implicit feedback received, so I guess they can improve the approach even more.

Finally, I liked that they shed some light into which cases the model recommends better, by segregating by popularity on users and shows. I think these kind of insights are important to improve the model. Even more, they presented some ideas on how to improve the performance.

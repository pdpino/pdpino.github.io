---
layout: post
title:  "Explanations on visual recommender"
date:   2019-10-13 10:00:00 -0300
categories: week9
week: "9"
---

**Paper:** Dominguez, V., Messina, P., Donoso-Guzmán, I., & Parra, D. (2019). The effect of explanations and algorithmic accuracy on visual recommender systems of artistic images. In Proceedings of the 24th International Conference on Intelligent User Interfaces (pp. 408-416). ACM.
{: .paper-name}

Context
{: .subtitle}

The paper presents an study on the effects of explanation in a recommender system, in the context of artwork recommendation from the Ugallery website.
Specifically, they tested multiple interfaces with different ways of explaining the recommendations, and two different content-based algorithms, the first using deep-learning and the second using manually-curated visual features.
The deep learning model has shown better accuracy on the recommendations, though is more opaque on the explanation; whilst the visual features approach has lower accuracy, but is highly transparent, since the features can be understand by humans.

Overall, I liked the user-centric approach.
In general, improving the user satisfaction should be the goal of recommender systems, but researchers mainly use offline metrics as a proxy of the performance.
In this work, they measure different aspects of the recommender interface, such as understandability, trust, or cognitive load, they test it with actual users, and they study quantitatively how those aspects influence the user satisfaction.

Baseline model?
{: .subtitle}

They could have added a baseline model to the tests.
Even though the goal was to compare the effects of explanations, they could have also tested a baseline model, such as Most Popular Artist or Favorite Artist, which have a very simple explanation (_"this is from the most popular artist"_ and _"this is from your favorite artists"_).
Then, in the analysis, they could have also determined if the proposed models are perceived better in terms of explainability, relevance, etc. compared to the simple baseline models, and concluded if the models actually improve the user satisfaction or not.

Art knowledge
{: .subtitle}

Regarding the AVF model, I think that the visual features listed are more useful to people who have at least some knowledge about art.
Someone with zero art knowledge (like me), wouldn't find the different features useful.
Accordingly, they could have differentiate the study results by art knowledge of the user.
Maybe, art experts perceive a better explanation or trust more on the AVF recommendations, opposed to non-expert users.


Also, they could have explicitly included in their study people who have actually bought art in Ugallery, and compare the results on that aspect.
Furthermore, it would be interesting to study the different methods on the real Ugallery website.
The actual interface may need to be simplified, or show a summarized explanation first, and only provide more details on demand of the user.
Then, the user satisfaction could be also estimated with click-through rate, session-time or other proxies, and even the revenue of the site could be evaluated.

Emergent artists
{: .subtitle}

Finally, they mention that UGallery supports emergent artists, so probably one of the most important aspects for the company could be the diversity of the recommendations.
Could the system provide an explanation of the diversity?
For instance, adding _"this is a new artist"_ to the explanation, when applicable.
Would this improve the diversity of purchased items?
Or people would tend to not buy the ones from new artists?
Since this is an important issue for Ugallery, I think it would be interesting to study it.

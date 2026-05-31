Project 1: Customer Segmentation using K-Means Clustering

The whole idea is simple — you have a list of customers and you want to group them by similarity. Not by guessing, not by manually sorting them, but by letting an algorithm figure out the natural groups hiding in your data.

Imagine you run a retail store. You have hundreds of customers but you treat them all the same — same emails, same promotions, same messaging. That's inefficient. Some customers spend a lot but come in rarely. Others spend little but come in every week. Some are young, some are older, some are price-sensitive, some aren't. K-Means finds those natural groupings automatically.

Here's how it works. You feed it your customer data — things like age, annual income, how much they spend, how often they visit. You tell it one thing upfront: how many groups you want. Let's say 4. The algorithm then places 4 random center points in your data, assigns every customer to their nearest center, recalculates where the centers should be based on who's in each group, and keeps repeating that process until the groups stop changing. What you're left with are 4 distinct customer segments — each one internally similar, and different from the others.

The tricky part is knowing what number to pick for K. That's where the Elbow Method comes in — which is exactly what that code in Cell 4 was doing. You run K-Means for every value of K from 1 to 10, score how tight the clusters are each time, plot it, and look for the elbow — the point where adding more clusters stops making a meaningful difference. That kink in the curve tells you the sweet spot.

The most important thing to understand about this project is that it is unsupervised learning — you never tell the algorithm what the groups should be. There are no right or wrong answers provided upfront. It discovers the structure in the data entirely on its own. That's what makes it fundamentally different from Project 2, where you're training on data where you already know the answers.

In the real world this is used everywhere — airlines grouping passengers into loyalty tiers, Netflix grouping viewers by taste, banks grouping customers by financial behavior, hospitals grouping patients by risk profile. Any time a business wants to stop treating everyone the same and start personalizing — this is the tool they reach for.

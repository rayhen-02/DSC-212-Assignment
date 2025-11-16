🥋 **Community Detection on Zachary’s Karate Club**

Spectral Modularity Bisection + Centrality Evolution Tracking

This project applies a spectral modularity community detection algorithm to the well-known Zachary’s Karate Club network. Beyond producing final communities, it also analyzes how node-level centrality measures change during each recursive split.

🔍 Key Features

Modularity Matrix (B) for global and subgraph splits

Recursive spectral bisection using the leading eigenvector

Per-iteration tracking of:

Degree Centrality

Betweenness Centrality

Closeness Centrality

Clustering Coefficient

Graph evolution visualizations with fixed layout and community colors

Metric evolution plots showing how node importance changes over time

Final community summary with sizes and average metrics

📘 Method Overview

The implementation follows Newman’s modularity maximization algorithm:

Start with the full graph as a single community.

Compute the refined modularity matrix 
𝐵
(
𝐶
)
B(C) of a subgraph.

Find the largest eigenvalue and leading eigenvector.

If the eigenvalue > 0, split nodes by eigenvector sign (+ / –).

Push resulting subcommunities back into the queue.

Continue until no split increases modularity.

📊 Result Summary

Final Communities: 5

Successful Splits: 4

First split clearly separated the two factions led by Node 0 and Node 33.

Later splits identified smaller cohesive subgroups and isolated outliers.

🧠 Centrality Insight

Betweenness centrality showed the most dramatic change:

Nodes 0 and 33 began as global brokers linking factions.

After the first split, their betweenness dropped sharply, revealing a transition to local leaders within isolated communities.

🧾 Conclusion

This project demonstrates that node importance is not static. Centrality values are structurally dependent and shift as the network moves from a global view to smaller, more cohesive communities. Community detection is therefore not only about where nodes belong, but also how their roles evolve.

📚 References

Algorithm:
Newman, M. E. J. (2006). Modularity and community structure in networks. PNAS, 103(23), 8577–8582.

Dataset:
Zachary, W. W. (1977). An information flow model for conflict and fission in small groups. Journal of Anthropological Research, 33(4), 452–473.



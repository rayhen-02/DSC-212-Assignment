# DSC-212-Assignment
Project Summary (Concise)

This project applies spectral modularity bisection to detect communities in Zachary’s Karate Club graph, while tracking how node centrality measures change during recursive splits.

Core Work Completed

Constructed the global and subgraph modularity matrix.

Implemented recursive spectral bisection using the leading eigenvector.

Tracked, at each split step:

Degree

Betweenness

Closeness

Clustering coefficient

Visualized:

Graph evolution (“time-lapse” community splits)

Metric evolution line plots for all nodes

Produced a final summary table and interpretation.

Algorithm Basis

Follows the modularity maximization method from Newman (2006) using eigenvectors of the modularity matrix B, applied recursively to subcommunities. Dataset from Zachary (1977).

Process Overview

Begin with the entire graph as one community.

Compute subgraph modularity matrix.

Get the largest eigenvalue and eigenvector.

If eigenvalue > 0, split based on vector signs; otherwise mark as final.

Continue until no further splits improve modularity.

Results & Key Insights

Final output: 5 communities formed over 4 successful splits.

First split separated the two historic factions (around Node 0 and Node 33).

Betweenness centrality revealed major role shifts:

Leaders (0 and 33) began as high-betweenness brokers.

Their betweenness dropped to near zero after separation, reflecting their shift to local community leaders.

Demonstrated that node importance is context-dependent and changes as the network is partitioned.

Final Conclusion

Community detection is not only about finding groups, but understanding how node roles evolve as structure becomes more localized. This project shows that centrality is dynamic, not fixed, and depends on the level of community resolution at which the network is studied

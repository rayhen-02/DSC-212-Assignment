**Karate_club_graph_Modularity**

This project aims to find the hidden communities in a real world dataset( Zachary's Karate Club network) using spectral bipartition algorithm and doing it recursivly.

**The Story Behind**

In the early 1970s, a graduate student in anthropology, Wayne W. Zachary, became interested in how friendships and alliances form within small social groups. To study this in detail, he spent two years observing the social interactions among 34 members of a university karate club in the United States. He carefully recorded who spent time with whom outside of formal classes: attending social events together, training together, and interacting as friends. These observations produced a network where each member of the club is a node, and an edge is drawn between two nodes if the members frequently interacted. This network, now called the Karate Club graph, is one of the most famous real-world social networks in network science. A twist in the story makes this dataset especially interesting. During Zachary’s fieldwork, the club’s instructor and the club’s administrator had a serious disagreement about whether club revenues should be spent on equipment or used for instructor salaries. This dispute escalated, eventually splitting the club into two rival factions. Members had to decide whom to follow: the instructor (“Mr. Hi”) or the administrator (the club president). Remarkably, the friendships Zachary had recorded before the split were strong predictors of how the split actually happened: friends tended to stick together. From a learning perspective, this network is a perfect case study. We know the “ground truth” outcome (two groups), but the network data were collected before the split occurred. This allows us to ask: Can a community-detection method, applied only to the graph structure, recover the division that actually happened? In other words, can we use mathematics to uncover the social fault lines that were about to fracture the club? Lets see !


**Reference:**

Based on Newman's 2006 paper on modularity and community structure. Uses the classic Zachary Karate Club dataset from 1977.

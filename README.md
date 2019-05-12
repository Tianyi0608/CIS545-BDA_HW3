# CIS545-BDA_HW3
Page rank (𝑃𝑅(𝑖)=𝛼⋅𝑀⋅𝑃𝑅(𝑖−1)+𝛽⋅[1,1,1,…]𝑇) 
1. Compute the weight transfer matrix M based on the algorithm: (𝑀[𝑖,𝑗]=1/nj, if 𝑛𝑗>0 and 𝑀[𝑖,𝑗]=0 otherwise)
2. Compute the page rank using the formula: 𝑃𝑅(𝑖)=𝛼⋅𝑀⋅𝑃𝑅(𝑖−1)+𝛽⋅[1,1,1,…]𝑇 and an iteration times
3. Explore the influences of page rank: the number of outgoing links, the incoming links from different subranges, overlapping in incoming and outgoing links

Results: 1. only adding outgoing links to a page does not contribute to the page rank, because nothing links to the page, it will loss scores but does not earn scores every iteration. 2. adding influential pages as incoming link increase page rank. 3. overlap the outgoing and incoming links benefit the page rank

____________________________________________________________________________________________________________________________

Transitive Closure based on BFS algorithm on Spark (given a set of nodes, compute the set of all nodes reachable from these nodes)
1. Set up the Google Spark environment
2. Upload data to Google Spark
3. Compute the transitive closure graph based on BFS

Important: the use of shuffle (repartition) and cache in Spark

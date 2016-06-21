---
title: "linear mapping"
bg: turquoise
color: white
fa-icon: map-o
---

### Considerations for Linear Mapping in Indoor Space

1. To partition indoor spaces into cells recursively
2. To reflect indoor distance matric
3. To assign a high priority to cluster objects in the same cell
4. To minimize sume of indoor distance


### Linear mapping using H-Graph

Partitioning and generating H-Graph

![H-Graph]({{ site.url }}/img/hgraph.png)


Linear mapping algorithm

- Traverse all nodes from the root node
- For each subgraph
  - Find candidates of orderings with the minimum sum of indoor distance
  - Choose the ordering connected to outer edges

![Linear mapping]({{ site.url }}/img/linearmapping.png)

![Linear mapping result]({{ site.url }}/img/linearmapping2.png)



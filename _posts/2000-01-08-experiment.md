---
title: "experiments"
bg: blue
color: white
fa-icon: bar-chart
---


## Summary of Experiments

- Characteristics of H-Graph
  - Comparison of depth
  - Comparison of average bf
  - Comparison of shapes with visualization
- Analysis of resilience against attacks
  - Comparison of success rate of center-of-ASR attack
  - Comparison of inference probability of replay attack
  - Comparison of success rate of replay attack
- Analysis of location K-anonymity at the anonymizer
  - Comparison of areas of ASR
  - Comparison of counts of cells
  - Comparison of the number of doors of ASR
- Analysis of query processing with the ASR at the LSP
  - Comparison of the number of candidates
  - Comparison of response time
- Analysis of linear mapping
  - Comparison of the number of jumps
  - Comparison of distance of jumps


## Experiment Setup

#### **Feature of LAB313 buiding dataset**

|     Attributes     | Values |
|:------------------:|:------:|
| # of subspaces     |   302  |
| # of floors        |    7   |
| avg. area of cells |  30.8m |
| var. area of cells |  95.8m |
| avg. degree        |   2.4  |
{: .striped .center}

![Building]({{ site.url }}/img/basegraph.png)
{: .center}

#### **Feature of Avenuel building dataset**

|     Attributes     | Values |
|:------------------:|:------:|
| # of subspaces     |   703  |
| # of floors        |    6   |
| avg. area of cells |  70.6m |
| var. area of cells |  90.5m |
| avg. degree        |   2.2  |
{: .striped .center}


![Lotte]({{ site.url }}/img/lotte.png)
{: .center}

-------------------------

#### **Summary of parameters for experiments**

|      Parameters     |           Values          |
|:-------------------:|:-------------------------:|
| Number of users     |  200, 400, 600, 800, 1000 |
| Anonymity degree K  |     5, 10, 15, 20, 25     |
| Diversity degree l  |    1, 5, 10, 15, 20, 25   |
| Anonymity method    |    KAH, KAHR, KAM, KAO    |
| H-Graph algorithm   | ControlValue, Count, Area |
| Range query param r |     5, 10, 15, 20, 25     |
| NN query param k    |     5, 10, 15, 20, 25     |
{: .striped .center}

-------------------------


## Characteristics of H-Graphs

![Experiment 1]({{ site.url }}/img/experiment-1.png)

-------------------------


## Analysis of Resilience against Attacks

![Experiment 2]({{ site.url }}/img/experiment-2.png)
![Experiment 3]({{ site.url }}/img/experiment-3.png)

-------------------------

## Analysis of K-Anonymization at the Anonymizer


![Experiment 4]({{ site.url }}/img/experiment-4.png)
![Experiment 5]({{ site.url }}/img/experiment-5.png)

---

## Analysis of Query Processing with the ASR at the LSP

![Experiment 6]({{ site.url }}/img/experiment-6.png)
![Experiment 7]({{ site.url }}/img/experiment-7.png)

---

## Analysis of Linear Mapping

![Experiment 8]({{ site.url }}/img/experiment-8.png)
![Experiment 9]({{ site.url }}/img/experiment-9.png)







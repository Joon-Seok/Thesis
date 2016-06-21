---
title: "anonymity"
bg: '#63BD2F'
color: white
fa-icon: user-secret
---

## System Model

We imploy a trusted third party (TTP) system between clients and LSPs to support location K-anonymization. The process consists of the following four steps.

1. A client sneds an original spatial query, which specifies the client's point location, to the anonymizer.
2. The anonymizer alters the query and delivers the modified query with ASR, cloaking the client's location, to the LSP
3. The LSP performs the query and returns candidates that are a super set of the actual results.
4. The anonymizer filters out candidates and sends back the actual results to the client.


![system architeucture]({{ site.url }}/img/system_architecture.png)

## Requirements for ASR Extension

1. Resilience against attack
  - Center-of-ASR attacks
  - Replay attacks
  - Homogeneity attacks
2. Efficiency of query processing
  - Preserving spatial locality
  - Small ASR
  - Avoiding fragmentation

## ASR Determination

Hierarchical graphs (H-Graph) are a proper data structure to reflect indoor characteristics. Thus, we employ the hierarchical structure of an indoor space for indoor location K-anonymization. We suggest three methods to determine the ASR with consideration of the requirements.

1. K-anonymity using H-Graph (KAH)
2. K-anonymity using H-Graph by random selection (KAHR)
3. K-anonymity on cell ordering using H-Graph (KAO)

### KAH

In order to satisfy K-anonymity, extend ASR from the leaf node where the requester is located.

<img src="{{site.url}}img/kah.png">


### KAHR

In order to reduce exponential enlargement of ASR of KAH, randomly select cells in ASR of KAH.

![KAHR]({{ site.url }}/img/kahr.png)


### KAO

In order to ensure reciprocity

- Make globally consistent groups that contain users
- Each group consists of at least K users.

Process of KAO

1. Oragnize all buckets
2. Find the bucket the requester belongs to
3. Find all the cells containing users in the buckets
4. Unite the cells as an ASR 

![KAO]({{ site.url }}/img/kao.png)



# PageRank Estimation Engine

## Projection Description

A Python-based graph processing tool based to implement and evaluate two fundamental PageRank estimation algorithms on directed web graphs:  **Monte Carlo Stochastic Random Walks** and **Iterative Probability Distribution

---

## Algorithms Implemented 

### 1. Stochastic PageRank 
* Models a random traverse of a directed graph with a standard damping factor.
* Approximates stationary distribution via tracking the frequency of visits over a large sample of continous random walks.
 
### 2. Distribution-Based PageRank 
* Computes exact stationary probability distribution across all graph vertices iteratively using transition probabilities.
* Updates staste vectors simultaneously until reaches convergence threshold or max iterations are exceeded.
## Features

Implements two PageRank estimation algorithms:
Stochastic PageRank using random walkers. 
Distribution-Based PageRank using probability updates. 
Command-line interface to select the method and control parameters.
Displays top-ranked pages and their PageRank values.
Prints number of nodes and edges about the graph 

## Graph Data Format

Input files should represent directed edge lists formatted as whitespace seperate node pairs:

```text
source_node_id destination_node_id
0 1
0 2
1 2

## Commands

python page_rank.py school_web2024-1.txt -m stochastic -r 1000000 -n 10
 
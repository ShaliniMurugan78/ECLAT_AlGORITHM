 ## What is ECLAT?

ECLAT is an **association rule mining algorithm** used to find **frequent itemsets** in transactional datasets.  
Unlike Apriori, ECLAT uses a **vertical data format**, where each item is associated with a set of transaction IDs (TID set).

**Key idea:**  
> Support of an itemset = size of the intersection of its TID sets

## Learning Objectives

Through this project, I learned:

- How association rule mining works
- Difference between **horizontal vs vertical data formats**
- How ECLAT improves performance over Apriori
- How to calculate support using **set intersections**
- How **depth-first search (DFS)** is used to generate frequent itemsets
- Strengths and limitations of the ECLAT algorithm

## Workflow of ECLAT Algorithm

1. Load transactional dataset  
2. Convert data into **vertical format (item → TID set)**  
3. Set minimum support threshold  
4. Generate frequent 1-itemsets  
5. Recursively intersect TID sets to generate larger itemsets  
6. Prune itemsets that do not satisfy minimum support  

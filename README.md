# The Product Space — Network Analysis of Global Trade Complexity

[View full analysis](https://htmlpreview.github.io/?https://github.com/tommaso-accornero/product-space-analysis/blob/main/product_space_analysis.html)

A structural network analysis of the **Product Space** (Hidalgo et al. (2007)), 
reproducing and extending the original paper's findings using Python and NetworkX.

![The Product Space Network](images/product_space_network.png)

## What is the Product Space?

The Product Space is a network of 774 economic products where two products are 
connected if they are systematically co-exported by the same countries — reflecting 
shared productive capabilities. The structure of this network shapes a country's 
ability to diversify its economy: countries can only realistically move into 
products that are close to their existing capabilities.

## Analysis

The notebook covers:
- Network description and sparsity
- Degree distribution (linear and log-log scale)
- Degree assortativity and core-periphery structure
- Community detection via Louvain algorithm (35 communities, modularity = 0.76)
- Degree and betweenness centrality analysis
- Configuration model test for clustering coefficient (Z-score = 160.20)
- Network visualization colored by community

## Key Finding

The Product Space cannot be explained by a random null model. Its high clustering 
coefficient (0.43) sits 160 standard deviations above the configuration model 
baseline — confirming that the network reflects genuine productive capability 
structures, not statistical chance.

## Stack

Python · NetworkX · Pandas · NumPy · Matplotlib

## Data

Coscia, M. & Hidalgo, C.A. — The Product Space (SITC classification)  
Source: [icon.colorado.edu](https://icon.colorado.edu)

## References

Hidalgo, C.A., Klinger, B., Barabási, A.L., & Hausmann, R. (2007). The Product Space 
Conditions the Development of Nations. *Science*, 317(5837), 482–487. 
https://doi.org/10.1126/science.1144581

Coscia, M. (2012). The Product Space Dataset (SITC classification). 
https://www.michelecoscia.com/?page_id=223

Kolic, B. (2025). UC3M Networks Workshop. 
https://github.com/blas-ko/uc3m_networks_workshop_2025
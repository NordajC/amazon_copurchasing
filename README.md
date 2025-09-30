# Analysing the Amazon Co-purchasing Network

> This project is an investigation of the Amazon co-purchasing network. Using Gephi and NetworkX, we analyse the complex network to identify its properties, discover influential products, and understand community structures. The goal is to gain a deeper understanding of Amazon's marketing and recommendation strategies.

## Introduction

The field of digital media and social networks is rapidly expanding. This project navigates the complexity of the Amazon co-purchasing network—the system that recommends related products to customers. By analysing a large dataset of Amazon product relationships, we aim to understand how such a co-purchasing system works and the degree of accuracy within it.

## Dataset

The analysis is based on the Amazon co-purchasing network from **March 2, 2003**. The dataset was cleaned to remove unrelated or unwanted data, ensuring more accurate results.

* **Nodes**: Represent individual products on Amazon.

* **Directed Edges**: Represent a co-purchase relationship (i.e., one product being frequently bought with another).

## Methodology

We employed a set of network analysis methods and tools to investigate the network's structure and dynamics.

### Tools Used

* **Gephi**: A powerful network visualization and exploration tool used for calculating network metrics, visualizing communities, and applying layout algorithms like Force Atlas 2.

* **NetworkX**: A Python library used for applying the PageRank algorithm to identify influential products within the network.

### Analysis Techniques

1. **Network Property Analysis**: We calculated key network metrics:

   * **Degree Distribution**: To understand the connectivity of products.

   * **Average Path Length**: To measure the average number of steps between any two products.

   * **Clustering Coefficient**: To evaluate the degree to which products form clusters.

2. **PageRank Analysis**: We used the PageRank algorithm to assign an importance score to each product, identifying those that are most central to consumer purchasing patterns.

3. **Community Detection**: Using Gephi's modularity tool (which applies the Louvain method), we identified distinct "communities" or clusters of products that are frequently purchased together.

## Results and Discussion

Our analysis revealed several key characteristics of the Amazon co-purchasing network.

### Network Type: Small-World Properties

The network exhibits the classic properties of a **small-world network**:

* **High Clustering Coefficient**: Calculated at **0.360**. This indicates that products tend to form tightly-knit groups or communities.

* **Short Average Path Length**: Calculated at **4.226**. This is significantly shorter than a comparable random network, indicating high navigability and efficient connections between products.

These properties enable efficient product discovery and specific recommendations but also introduce vulnerabilities, such as an over-reliance on central hub products.

### Key Findings

* The network follows a **heavy-tail degree distribution**, meaning a few products (hubs) have a very high number of connections, while most products have very few.

* The small-world structure allows for the rapid spread of information (like recommendations or reviews) but also creates risks, such as echo chambers or the rapid spread of negative content.

* Products with high PageRank scores (e.g., Product ID `8`, `33`, `93`) are influential hubs in the network and are central to purchasing dynamics.

## Conclusion

The Amazon co-purchasing network is a small-world network that enables efficient recommendations but also has structural vulnerabilities due to its reliance on central hubs. By identifying influential products and community structures, we can derive insights to refine marketing strategies, enhance network resilience, and improve the customer experience by introducing more diverse recommendations.

## Authors

* Noshad Boksh

* Jun Hann Chong

* Remy Philip Jean MacDermott

* Senthuran Krishnakumar

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

* **NetworkX**: A Python library used for applying the PageRank algorithm to identify influential products within

# Social Media Influence Analysis

This repository contains the first semester project for the course "22MAT121: Discrete Mathematics".

## Problem Statement
The project aims to comprehensively analyze the dissemination of information on social media platforms, focusing primarily on Facebook. Through the utilization of graph theoretical methods and machine learning techniques, the project endeavors to unravel the intricate dynamics of social media influence and interactions within digital networks.

## Objectives
- Conduct in-depth analysis of social media data using graph theory and machine learning.
- Visualize network structures to gain insights into the relationships between Facebook accounts.
- Calculate centrality measures to identify influential nodes and understand their significance within the network.
- Perform statistical analysis to quantify various aspects of the dataset and reveal trends, patterns, and anomalies.
- Utilize community detection techniques to uncover clusters and patterns of interactions within different categories of Facebook pages.
- Characterize Facebook pages based on features and network structure to understand their roles and behaviors within the network.

## Datasets Used
The project leverages Facebook datasets obtained from the [Snap Stanford repository](http://snap.stanford.edu/data/gemsec-Facebook.html). These datasets consist of CSV files capturing interactions between Facebook accounts, along with a JSON file providing additional attributes for each account.

## Methodology
1. **Graph Visualization:** Utilize NetworkX to visualize network structures, representing Facebook accounts as nodes and interactions as edges.
2. **Centrality Analysis:** Calculate degree centrality, closeness centrality, and betweenness centrality to identify influential nodes within the network.
3. **Statistical Analysis:** Conduct statistical analysis to quantify various aspects of the dataset, including the number of nodes, edges, average degree, and clustering coefficient, providing insights into the structural dynamics of different categories of Facebook pages.
4. **Community Detection:** Employ community detection techniques to uncover clusters of nodes with dense intra-cluster connections, revealing patterns of interactions within different categories of Facebook pages.
5. **Page Characterization:** Use machine learning techniques like RandomWalk to characterize Facebook pages based on features and network structure, providing insights into their roles and behaviors within the network.

## Implementation
The project is implemented using Python programming language, with the aid of libraries such as Pandas, Numpy, NetworkX, Matplotlib, scikit-learn and Gensim. Code files and datasets are included in the repository for replication and further analysis.

## Results
The results section provides a detailed analysis of the findings obtained from each stage of the methodology:
- **Graph Visualization:** Effectively portrays network structure, with nodes representing unique users/accounts and edges revealing connections.
- **Centrality Measures:** Provided insights into individual accounts' structural dynamics and influence within respective categories.
- **Statistical Analysis:** Revealed structural insights; "Companies" emerged with highest node count, "Government" with most edges and highest average degree and clustering coefficient.
- **Community Detection:** Unveiled distinct clusters within each category; "Government" exhibited 22 communities, "TV Shows" displayed 60 communities, "Company" presented 195 communities, and "Politician" showed 36 communities.
- **Page Characterisation:** Achieved testing accuracy of 0.9096573208722741, indicating effectiveness in classifying Facebook pages based on features and network attributes.

## Conclusion
In conclusion, the project contributes to a deeper understanding of social media influence and interactions on Facebook. By employing a comprehensive methodology encompassing graph theory, machine learning, and statistical analysis, the project provides valuable insights into the dynamics of social media networks and their implications for digital communication and influence.

## Contributors
- Shruti Sivakumar
- Harshitha Chandrasekar
- Shreya Sriram
- Vida Nadheera

## License
This project is licensed under the terms of the MIT License. See the [LICENSE](LICENSE) file for details.

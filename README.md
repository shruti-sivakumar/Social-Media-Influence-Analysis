# Social Media Influence Analysis

This project presents an exploration of social media networks using graph theory and machine learning during my early stages of university. By analyzing Facebook page interactions from the [SNAP dataset repository](http://snap.stanford.edu/data/gemsec-Facebook.html), it investigates influence dynamics, network structure, and page behavior using advanced network science techniques.

---

## Problem Statement

Understanding how information spreads across social media platforms is essential for applications in crisis response, marketing, and public engagement. This project models information flow as a graph problem, with accounts as nodes and interactions (e.g., mutual likes) as edges. Through a layered approach involving centrality, community detection, and node classification, the project identifies influential structures and behavioral patterns in verified Facebook networks.

---

## Objectives

- Analyze social media data using **graph-theoretic and ML techniques**
- Visualize Facebook network structures and interpret interaction patterns
- Identify influential nodes via **centrality metrics** (degree, closeness, betweenness)
- Quantify structural characteristics via **statistical analysis**
- Detect community structure using **greedy modularity-based clustering**
- Characterize pages using **graph embeddings (RandomWalk/Node2Vec)** and **Random Forest classification**

---

## Datasets Used

From SNAP’s Facebook verified page dataset (2017), categorized by page type:
- **Files**: `*_edges.csv` (edge lists per category), `dataset_descriptions.txt`
- **Categories**: Government, Politicians, Companies, TV Shows, Artists, Athletes, Public Figures, News Sites
- **Format**: Each edge represents mutual page likes between `node_1` and `node_2`

---

## Methodology

### 1. Graph Visualization
- Construct graphs with NetworkX using edge lists
- Spring layout visualization with custom styling
- Nodes represent pages; edges represent mutual likes

### 2. Centrality Analysis
- Compute **Degree Centrality**: measures popularity (number of connections)
- Compute **Closeness Centrality**: measures reachability across network
- Compute **Betweenness Centrality**: identifies bridges and flow controllers

### 3. Statistical Analysis
- Number of nodes and edges
- Average degree: network density
- Clustering coefficient: degree of triadic closure

### 4. Community Detection
- Use **Greedy Modularity Optimization** to find dense clusters within categories
- Visualize communities using subgraph spring layouts
- Report number of communities per category

### 5. Page Characterization (ML)
- Use **RandomWalk-based Word2Vec** embeddings for structural feature learning
- Train **Random Forest Classifier** on learned embeddings to predict page type
- Evaluate using accuracy, confusion matrix, F1 score

---

## Result Highlights

| Category     | Nodes | Edges  | Avg Degree | Clustering Coef | Communities |
|--------------|-------|--------|-------------|------------------|-------------|
| Government   | 7057  | 89455  | 25.35       | 0.41             | 22          |
| TV Shows     | 3892  | 17262  | 8.87        | 0.37             | 60          |
| Company      | 14113 | 52310  | 7.41        | 0.24             | 195         |
| Politicians  | 5908  | 41729  | 14.13       | 0.39             | 36          |

**Page Classification Accuracy**: **90.96%** using Random Forest on structural embeddings.

> Outputs are present directly in the Jupyter notebooks.

---

## Repository Structure

```
├── data/
│   └── facebook_clean_data/       # Raw edge lists per category
    ├── dataset_description.txt
├── notebooks/
│   ├── 1_graph_visualization.ipynb
│   ├── 2_centrality_analysis.ipynb
│   ├── 3_statistical_analysis.ipynb
│   ├── 4_community_detection.ipynb
│   └── 5_page_characterisation.ipynb
├── LICENSE
└── README.md
```

---

## Conclusion

This project demonstrates the effective application of discrete mathematics and network science to real-world social media data. By combining classical centrality analysis with modern graph embeddings and ML classification, it provides a holistic understanding of influence dynamics and page behavior in Facebook’s verified page ecosystem.

The multi-stage pipeline—spanning visualization, statistical analysis, community clustering, and predictive modeling—offers a versatile framework for social network analysis. Future extensions may involve temporal dynamics, multi-platform integration, and Graph Neural Networks.

---

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file.

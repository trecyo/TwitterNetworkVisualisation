# **Twitter Network Analysis: June 2025 Kenya Protests**

This project provides a macro-level visualization and social network analysis (SNA) of the digital discourse surrounding the Kenya protests in June 2025. By analyzing the structural properties of the Twitter (X) network, this study identifies key influencers, information brokers, and community clusters.



### Dataset Overview

The visualization is built upon a large-scale directed graph representing interactions (retweets, mentions, and replies) during the peak of the protests.



Nodes: 15,969 (Unique users)



Edges: 41,518 (Interactions)



Type: Directed Network



### Methodology \& Tools

The analysis was performed using Gephi 0.10.1. To make sense of the dense interaction data, the following layout and metrics were applied:



#### Network Topology

Layout Algorithm: ForceAtlas 2. To manage the high density of the core, a Scaling of 10,000.0 was applied to increase the distance between hubs, combined with Gravity (1.0) to maintain network cohesion.



Cleanup: Used Expansion and Noverlap passes to ensure label readability for high-centrality nodes.



#### Graph Metrics

Average Clustering Coefficient: 0.008 (Indicative of a highly dispersed, wide-reaching information flow rather than isolated "echo chambers").



Modularity: Used to detect distinct community clusters within the protest movement.



Centrality Measures: Node size is ranked by Betweenness Centrality to highlight "bridge" accounts that controlled the flow of information between different social groups.



### Key Findings

Influence Mapping: Identified the top 15 most influential accounts based on Betweenness Centrality. These accounts acted as the primary conduits for news and mobilization.



Sparsity: The low clustering coefficient suggests that the protest discourse was rapidly expanding across diverse networks rather than staying within a tight-knit circle of users.



#### Repository Structure

/data: Contains the (anonymized) edge and node lists.



/visualizations: High-resolution PDF and PNG exports of the final Gephi graph.



/reports: Detailed breakdown of the top 15 nodes and modularity reports.



### How to Replicate

Download the .gephi file from the /data folder.



Open in Gephi.



Run ForceAtlas 2 with the settings: Scaling: 10,000, Gravity: 1.0, Dissuade Hubs: True.



Run the Statistics panel (Average Path Length, Modularity, Clustering Coefficient) to regenerate the metrics.


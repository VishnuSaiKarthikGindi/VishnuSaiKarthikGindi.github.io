---
title: "MovieMagic: A Recommendation Engine"
excerpt: "Building a cutting-edge recommendation system using Graph Neural Networks (GCN and GAT) integrated with a Factorization Machine for predicting user-item interactions on the MovieLens dataset.<br/><img src='/images/MM.png'>"
collection: portfolio
---

### Description
In this project, the **MovieLens** dataset is used, containing user ratings of movies. The data was preprocessed by splitting into training and testing sets, where the latest interaction for each user was reserved for testing. An adjacency matrix was constructed to represent user-item interactions, and negative sampling was performed to create balanced training data.

The model was developed using **Graph Convolutional Networks (GCN)** and **Graph Attention Networks (GAT)** layers within the NGCF framework, implemented in PyTorch Geometric (PyG). These layers were combined with a **Factorization Machine (FM)**, which models second-order feature interactions. This integration captures both the graph structure and the latent relationships between users and items, offering a significant improvement over traditional collaborative filtering methods.

Compared to traditional methods, the developed model shows superior performance in recommendation tasks by effectively capturing higher-order connections in the data. The model was evaluated using HR and NDCG metrics, demonstrating substantial improvements in ranking quality, with HR increasing by up to 15% compared to baseline models.

You can view the full code and implementation details on [GitHub](https://github.com/VishnuSaiKarthikGindi/Recommendations_using_NGCF_and_PyG).

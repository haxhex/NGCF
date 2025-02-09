# Neural Graph Collaborative Filtering (NGCF)

## Overview  
This project implements the **Neural Graph Collaborative Filtering (NGCF)** model for recommendation systems using the **MovieLens-1M dataset**. NGCF leverages high-order connectivity and layer aggregation to improve the learning of user-item embeddings. The project includes model training, evaluation, and visualization of key metrics such as **Recall** and **NDCG**.

## Features  
- **Dataset:** MovieLens-1M dataset containing user-movie ratings.  
- **Model:** Neural Graph Collaborative Filtering (NGCF) for capturing higher-order relationships.  
- **Optimization:** Bayesian Personalized Ranking (BPR) loss for ranking-based learning.  
- **Evaluation:** Recall and NDCG metrics to assess recommendation performance.  
- **Visualization:** Loss-epoch plots to monitor training progress.

## Dataset  
The MovieLens-1M dataset, containing 1 million ratings from users on various movies, can be downloaded [here](https://huggingface.co/datasets/reczoo/Movielens1M_m1/tree/main). The dataset includes user information, movie metadata, and rating interactions.

**Loss and Metric Visualization:** The notebook provides plots of loss over epochs and evaluates Recall/NDCG performance.

## Optimization and Loss Function  
NGCF uses the **Bayesian Personalized Ranking (BPR) loss**, which optimizes embeddings by focusing on the relative ordering of observed and unobserved interactions. This enhances recommendation quality by prioritizing relevant items in ranking tasks.

## Layer Aggregation Mechanism  
The NGCF model aggregates embeddings from different propagation layers to capture multi-level interactions between users and items. This mechanism improves recommendation performance by combining low-order and high-order connectivity information.

## Results  
- **Evaluation:** Recall and NDCG scores for different training epochs.  
- **Loss Visualization:** Training loss curves help monitor convergence and overfitting.  
- **Embedding Analysis:** Discussion on how embedding smoothness and generalization affect performance.

## Future Improvements  
- Introducing attention mechanisms for adaptive neighbor weighting.  
- Experimenting with regularization techniques to enhance model robustness.

## References  
- **Paper:** [Neural Graph Collaborative Filtering](https://arxiv.org/abs/1905.08108) by Wang et al.  
- **Dataset:** [MovieLens-1M](https://grouplens.org/datasets/movielens/1m/)

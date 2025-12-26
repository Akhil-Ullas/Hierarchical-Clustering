✔ A Short Overview of Hierarchical Clustering

Hierarchical Clustering is an unsupervised learning technique that builds clusters in the form of a tree-like structure (dendrogram), allowing data to be grouped:

• progressively (step-by-step)
• at different granularity levels
• without pre-specifying the number of clusters

Unlike partition-based methods such as K-Means, hierarchical clustering focuses on relationship structure, not just compact grouping.

📌 Agglomerative vs Divisive Clustering

The module primarily focused on:

🔹 Agglomerative Clustering (Bottom-Up)
• each point starts as an individual cluster
• similar clusters are merged step-by-step
• process continues until a single cluster remains

(used in most practical applications)

🔹 Divisive Clustering (Top-Down)
• all points start in one cluster
• recursively split into smaller clusters

This provided deeper intuition into how cluster trees evolve over time.

📌 Linkage Methods Explored

I experimented with different linkage strategies to understand how distance influences cluster merging:

• Single Linkage — nearest-neighbor merging
• Complete Linkage — farthest-neighbor merging
• Average Linkage — mean distance merging
• Ward’s Method — variance-minimizing merging

Each linkage style produced different cluster shapes, separations, and interpretations, reinforcing the importance of selecting linkage based on data behavior rather than default settings.

✔ Key Concepts & Insights Gained

• Role of distance metrics in clustering
• Effect of scaling & normalization on structure
• Cluster granularity vs interpretability
• Choosing cut-levels on the dendrogram
• Trade-offs between compactness & hierarchy depth

I also compared how clusters changed when:

• features were rescaled
• distance metrics were modified
• linkage strategies were altered

This strengthened my understanding of cluster stability and robustness.

📌 Dendrogram Interpretation

One of the most valuable outcomes was learning to interpret dendrograms to:

• identify natural breakpoints
• observe merging behavior
• understand similarity relationships
• infer hierarchical group structure

Instead of selecting a fixed K, I evaluated:

• where meaningful cluster separation emerged
• whether clusters were dense, overlapping, or fragmented

✔ Applications Where Hierarchical Clustering Is Useful

• Customer & behavior segmentation
• Social grouping & similarity analysis
• Document or gene similarity mapping
• Hierarchical category discovery
• Feature grouping in preprocessing pipelines

It proved especially insightful when cluster relationships mattered more than labels.

✔ Advantages Observed

• No need to pre-define number of clusters
• Provides a full hierarchy instead of a single solution
• Useful for exploratory data analysis
• Dendrograms make structure visually interpretable

✘ Limitations Acknowledged

• Computationally expensive for large datasets
• Sensitive to noise and scaling
• Difficult to revise once clusters are merged
• Results vary significantly with linkage choice

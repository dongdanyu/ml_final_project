---
output:
  pdf_document: default
  html_document: default
---
# STA 380
## Fangshu Song, Siyi Liu, Vishal Dupta, Yu Xia


## Probability practice

__Part A.__ 


__Part B.__ 



## Wrangling the Billboard Top 100  

__Part A__:    



__Part B__: 



__Part C__: 



## Visual story telling part 1: green buildings


## Visual story telling part 2: Capital Metro data



## Clustering and dimensionality reduction  

I have conducted a thorough analysis of the vinho verde wine dataset using dimensionality reduction techniques (PCA and t-SNE) as well as K-Means clustering. The code and visualizations can be found in
<a href="https://github.com/dongdanyu/ml_final_project/blob/main/clustering_dimensionality_reduction/clustering.ipynb">Clustering and dimensionality reduction</a>

**Principal Component Analysis (PCA):**

Upon applying PCA to the standardized chemical properties, I visualized the results in the PCA plot does indeed show clusters forming based on the wine type (red and white). However, there is an observation to be made regarding the structure of the clusters. The red clusters and the blue cluster borders appear to be attached together, with limited separation. This suggests that while PCA does exhibit some level of clustering.

![pca](/clustering_dimensionality_reduction/diagram/pca.png)


**t-Distributed Stochastic Neighbor Embedding (t-SNE):**

In contrast, t-SNE revealed remarkable results in the t-SNE plot demonstrates a different outcome. Here, the red clusters and the blue cluster borders are visually separated, with a distinct gap in the middle. This separation is a notable feature of the t-SNE visualization and indicates a clearer distinction between red and white wines based on their chemical properties.


![tsne_type](/clustering_dimensionality_reduction/diagram/tsne_type.png)

While both PCA and t-SNE exhibit clustering tendencies, the unique separation exhibited by t-SNE further solidifies its effectiveness in distinguishing between red and white wines based on the unsupervised information contained in the data's chemical properties.

Furthermore, I employed t-SNE to create a plot that attempts to segregate wines based on quality. However, this particular plot does not exhibit a substantial separation between higher and lower quality wines. So my unsupervised technique cannot capable of distinguishing the higher from the lower quality wines

![tsne_qaulity](/clustering_dimensionality_reduction/diagram/tsne_quality.png)


**K-Means Clustering with t-SNE:**

The K-Means clustering plot shares a resemblance to the t-SNE plot. This similarity strengthens the notion that t-SNE captures the natural groupings effectively, as K-Means aligns with its outcomes.

![kmeans](/clustering_dimensionality_reduction/diagram/kmeans.png)
 
**Conclusion:**

Based on the analysis, it is evident that t-SNE is the most suitable dimensionality reduction technique for this dataset. It effectively separates red and white wines, showcasing its ability to distinguish categories with clear natural separation. However, it seems that the chemical properties alone may not be sufficient to distinctly cluster wines by quality. The K-Means clustering results further support the patterns observed in the t-SNE plot.


## Market segmentation

You can find the complete code and analysis in my GitHub repository: <a href="https://github.com/dongdanyu/ml_final_project/blob/main/market_segmentation/market.ipynb">Market Segmentation</a>

To begin the market segmentation, I conducted a correlation matrix analysis and visualized it as a heatmap. The heatmap revealed strong correlations between certain variables, such as "college_unit" and "online_gaming," as well as "personal_fitness" and "health_nutrition." Additionally, some moderate correlations, like 0.6 between "beauty" and "fashion," were observed.

![heatmap](/market_segmentation/heatmap.png)

Afterwards, I performed data preprocessing by dropping columns that weren't relevant for the segmentation analysis. These columns include 'chatter,' 'spam,' 'adult,' and 'Unnamed: 0.' The 'Unnamed: 0' column, which represents user names, was omitted since it doesn't contribute to the analysis. The other dropped columns contain an "uncategorized" label meant to capture posts that don't fit within the listed interest categories.

Next, I employed the K-Means clustering algorithm to uncover distinct market segments. I began by determining the optimal number of clusters (k) using the elbow method.

![kvalue](/market_segmentation/kvalue.png)

Based on the elbow method plot, I selected k=5 as the optimal number of clusters.

Subsequently, I generated a cluster plot that visually depicts the segments:

![cluster](/market_segmentation/cluster.png)


![clustervalue](/market_segmentation/clustervalue.png)


Upon analyzing the clusters, I derived the following summaries:

Cluster 0: This cluster seems to have a relatively high emphasis on topics related to "photo_sharing," "food," "parenting," and "personal_fitness," with moderate values for other topics. It could represent a cluster of users interested in lifestyle, parenting, and health-related content.

Cluster 1: This cluster has higher values for "politics," "sports_fandom," "automotive," and "dating," indicating potential interest in politics, sports, and dating-related topics.

Cluster 2: This cluster has higher values for "uncategorized," "beauty," "fashion," and "small_business," suggesting a focus on fashion, beauty, and potentially entrepreneurial content.

Cluster 3: This cluster shows significantly higher values for "religion," "parenting," "school," and "personal_fitness," indicating an interest in religious, parenting, educational, and health/fitness content.

Cluster 4: This cluster has relatively lower values across most topics, suggesting a more diverse range of interests without a strong focus on any specific topic.

In summary, the market segmentation analysis has uncovered five distinct clusters, each representing users with varying interests and preferences. These insights can be valuable for targeted marketing strategies and tailored content delivery.


## The Reuters corpus  



## Association rule mining




## Image classification with neural networks



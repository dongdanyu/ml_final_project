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


## The Reuters corpus  



## Association rule mining




## Image classification with neural networks



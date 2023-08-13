---
output:
  pdf_document: default
  html_document: default
---
# STA 380
## Fangshu Song, Siyi Liu, Vishal Anand Gupta, Yu Xia


## Probability practice

The detailed calculation steps for both parts can be found in 
<a href="https://github.com/dongdanyu/ml_final_project/blob/main/probability_practice/Probability Practice.ipynb">Probability Practice</a>.

__Part A.__ 

The fraction of people who are truthful clickers and answered "Yes" is approximately 0.7143 or 71.43%.

__Part B.__ 

The probability that a person has the disease given they tested positive is 0.00989 or 0.989%.


## Wrangling the Billboard Top 100  

The code and visualizations for part A, B and C can be found in 
<a href="https://github.com/dongdanyu/ml_final_project/blob/main/wrangling_billboard_top_100/Wrangling the Billboard Top 100.ipynb">Wrangling the Billboard Top 100</a>.

__Part A__:

The table below captures the essence of the top 10 most popular songs since 1958, meticulously curated based on their enduring impact and the total number of weeks they graced the esteemed Billboard Top 100 chart. Comprising a blend of genres and artists, the table encapsulates the musical journey of these songs that have left an indelible mark on the cultural fabric.

![top_100_songs](/wrangling_billboard_top_100/Top_10_most_popular_songs_since_1958.png)


__Part B__: 

The line chart below illustrates the evolution of "Musical Diversity" from 1959 to 2020, as measured by the number of unique songs released in each specific year. The trend showcases distinct phases of change, marked by periods of decline, recovery, and remarkable resurgence.

![Musical_Diversity](/wrangling_billboard_top_100/Musical_Diversity.png)

Some insights on the trend:

- In the early years, from 1959 to the late 1960s, the musical landscape was characterized by a diverse array of songs, reflecting a dynamic and experimental era in music production.
- The chart indicates a noticeable decline in musical diversity starting around 1968, persisting through the end of the 20th century.
- A brief period of recovery in the early 2000s is evident, indicating a renewed interest in experimenting with diverse musical styles.
- A remarkable and sustained increase in musical diversity is observable from around 2004 to 2011. This period could be associated with the rapid growth of the internet, streaming services, and social media, enabling artists from various backgrounds to gain visibility and reach a global audience.
- The last phase is from 2014 to 2020. The trend highlights a somewhat plateaued diversity after the substantial increase observed in the previous decade.

In summary, the trend of "Musical Diversity" over time reflects the dynamic interplay between technological advancements, industry shifts, and cultural influences.


__Part C__: 

The bar plot illustrates the achievements of 19 prominent artists in U.S. musical history since 1958, showcasing the number of their "ten-week hits." Each bar represents an individual artist, and its height quantifies the count of songs that remained on the charts for an impressive ten weeks or more. The data is thoughtfully sorted from the highest to the lowest count of ten-week hits, offering a clear perspective on the most prolific artists in terms of extended chart presence.

![Ten_Week_Hits_Artists](/wrangling_billboard_top_100/Ten_Week_Hits_Artists.png)

Some insights on the plot:
- The range of artists featured on the plot spans a wide spectrum of musical genres, attesting to the diverse musical talents that have shaped U.S. musical history.
- At the pinnacle of the plot, towering bars represent artists who have achieved extraordinary success in terms of ten-week hit songs. Elton John, for instance, stands out with an impressive count of 52 such hits, signifying his enduring popularity and influence across generations.
- The bar plot encapsulates the legacies of musical legends such as Michael Jackson and The Rolling Stones. Their counts of ten-week hits provide a glimpse into the enduring appeal and lasting impact of their contributions to music.

In summary, the bar plot not only showcases the achievements of artists in terms of ten-week hits but also offers a captivating narrative of the ever-evolving world of U.S. musical history.


## Visual story telling part 1: green buildings
code:
<a href="https://github.com/dongdanyu/ml_final_project/blob/main/greenbuildings%26capmetro_UT/ML.ipynb">green buildings</a>

## Visual story telling part 2: Capital Metro data

code:
<a href="https://github.com/dongdanyu/ml_final_project/blob/main/greenbuildings%26capmetro_UT/ML.ipynb">capmetro UT</a>


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



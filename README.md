# Clustering-Analysis-on-Estimation-of-obesity-levels-dataset

## Comparitive performance study of different clustering algorithms using different pre-processing techniques with different numbers of clusters on different evaluation parameters
- Select any small dataset from UCI library
- Create Colab notebook and perform cluster alaysis
- Upload on github and describe in brief with results, tables, graphs and conclusion and upload on github.

### Sample Result Table
![131206252-10a4e5ec-ec8f-4017-8617-ae46d47dcdcf](https://github.com/psrana/Clustering-Assignment/assets/7460892/8cd5f3d3-3891-4a9c-8c6e-9abfb8f0a946)

## Results for Estimation of obesity levels based on eating habits and physical condition  Dataset
### KMEANS
|name             |No Preprocessing|No Preprocessing|No Preprocessing|Norm + PCA|Norm + PCA|Norm + PCA|Norm + PCA + TRANS|Norm + PCA + TRANS|Norm + PCA + TRANS|Normalisation|Normalisation|Normalisation|PCA      |PCA      |PCA      |Transformation|Transformation|Transformation|
|-----------------|----------------|----------------|----------------|----------|----------|----------|------------------|------------------|------------------|-------------|-------------|-------------|---------|---------|---------|--------------|--------------|--------------|
|cluster_size     |3               |4               |5               |3         |4         |5         |3                 |4                 |5                 |3            |4            |5            |3        |4        |5        |3             |4             |5             |
|Silhouette       |0.5022          |0.474           |0.4297          |0.1821    |0.1415    |0.1761    |0.1539            |0.1617            |0.1584            |0.1812       |0.1402       |0.1579       |0.5022   |0.4739   |0.431    |0.7405        |0.7081        |0.6529        |
|Calinski-Harabasz|4716.4535       |4798.135        |4576.5499       |218.7888  |202.2217  |192.6706  |213.7715          |193.5156          |181.4668          |218.811      |202.2135     |192.8943     |4716.4535|4798.1522|4577.5126|91011.4113    |83222.2409    |93117.9441    |
|Davies-Bouldin   |0.6694          |0.7016          |0.7598          |2.2327    |2.3849    |1.8759    |2.417             |2.1783            |2.417             |2.2344       |2.381        |2.0834       |0.6694   |0.7022   |0.7516   |0.4023        |0.58          |0.5592        |


### meanshift
|name             |No Preprocessing|No Preprocessing|No Preprocessing|Norm + PCA|Norm + PCA|Norm + PCA|Norm + PCA + TRANS|Norm + PCA + TRANS|Norm + PCA + TRANS|Normalisation|Normalisation|Normalisation|PCA     |PCA      |PCA      |Transformation|Transformation|Transformation|
|-----------------|----------------|----------------|----------------|----------|----------|----------|------------------|------------------|------------------|-------------|-------------|-------------|--------|---------|---------|--------------|--------------|--------------|
|cluster_size     |3               |4               |5               |3         |4         |5         |3                 |4                 |5                 |3            |4            |5            |3       |4        |5        |3             |4             |5             |
|Silhouette       |0.5585          |0.5585          |0.5585          |0.285     |0.285     |0.285     |0.293             |0.293             |0.293             |0.285        |0.285        |0.285        |0.5585  |0.5585   |0.5585   |0.9448        |0.9448        |0.9448        |
|Calinski-Harabasz|4301.3718       |4301.3718       |4301.3718       |27.8296   |27.8296   |27.8296   |33.0076           |33.0076           |33.0076           |27.8296      |27.8296      |27.8296      |4301.3718|4301.3718|4301.3718|88381.1313    |88381.1313    |88381.1313    |
|Davies-Bouldin   |0.5994          |0.5994          |0.5994          |0.7848    |0.7848    |0.7848    |0.7795            |0.7795            |0.7795            |0.7848       |0.7848       |0.7848       |0.5994  |0.5994   |0.5994   |0.0998        |0.0998        |0.0998        |


### hclust

|name             |No Preprocessing|No Preprocessing|No Preprocessing|Norm + PCA|Norm + PCA|Norm + PCA|Norm + PCA + TRANS|Norm + PCA + TRANS|Norm + PCA + TRANS|Normalisation|Normalisation|Normalisation|PCA     |PCA      |PCA      |Transformation|Transformation|Transformation|
|-----------------|----------------|----------------|----------------|----------|----------|----------|------------------|------------------|------------------|-------------|-------------|-------------|--------|---------|---------|--------------|--------------|--------------|
|cluster_size     |3               |4               |5               |3         |4         |5         |3                 |4                 |5                 |3            |4            |5            |3       |4        |5        |3             |4             |5             |
|Silhouette       |0.4824          |0.4735          |0.4216          |0.1486    |0.167     |0.1394    |0.0954            |0.1251            |0.1472            |0.1486       |0.167        |0.1394       |0.4744  |0.4663   |0.4161   |0.7405        |0.7081        |0.6529        |
|Calinski-Harabasz|4368.6177       |4438.1771       |4183.4448       |192.5245  |177.645   |171.1922  |180.6725          |168.1934          |165.8775          |192.5245     |177.645      |171.1922     |4285.517|4326.8265|4132.3053|91011.4113    |83222.2409    |93117.9441    |
|Davies-Bouldin   |0.6925          |0.6618          |0.7339          |2.7343    |2.7231    |2.6463    |2.5312            |2.8816            |2.7323            |2.7343       |2.7231       |2.6463       |0.7022  |0.669    |0.745    |0.4023        |0.58          |0.5592        |


### dbscan

|name             |No Preprocessing|No Preprocessing|No Preprocessing|Norm + PCA|Norm + PCA|Norm + PCA|Norm + PCA + TRANS|Norm + PCA + TRANS|Norm + PCA + TRANS|Normalisation|Normalisation|Normalisation|PCA     |PCA      |PCA      |Transformation|Transformation|Transformation|
|-----------------|----------------|----------------|----------------|----------|----------|----------|------------------|------------------|------------------|-------------|-------------|-------------|--------|---------|---------|--------------|--------------|--------------|
|cluster_size     |3               |4               |5               |3         |4         |5         |3                 |4                 |5                 |3            |4            |5            |3       |4        |5        |3             |4             |5             |
|Silhouette       |-0.5602         |-0.5602         |-0.5602         |-0.2435   |-0.2435   |-0.2435   |-0.2754           |-0.2754           |-0.2754           |-0.2435      |-0.2435      |-0.2435      |-0.5602 |-0.5602  |-0.5602  |-0.4659       |-0.4659       |-0.4659       |
|Calinski-Harabasz|19.0544         |19.0544         |19.0544         |10.0541   |10.0541   |10.0541   |9.8477            |9.8477            |9.8477            |10.0541      |10.0541      |10.0541      |19.0544 |19.0544  |19.0544  |6.1981        |6.1981        |6.1981        |
|Davies-Bouldin   |1.2283          |1.2283          |1.2283          |1.4235    |1.4235    |1.4235    |1.4414            |1.4414            |1.4414            |1.4235       |1.4235       |1.4235       |1.2283  |1.2283   |1.2283   |1.6331        |1.6331        |1.6331        |


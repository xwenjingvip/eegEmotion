# 空间情感维度 => 离散情感维度
## 方案1：
+ DEAP数据集是四维的情感标签，这里需要将其向离散情感维度进行转化。我们选取三维度的Arousal-Valencee-Dominance情感空间对数据进行聚合
+ 使用K-means算法进行聚类：
  - 积极，消极中心点。以Valence维度上的'5'为分界，分别求取数据在VAD三个维度的中位数(平均值)，将其作为分类点。
  - 平静中心点：直接取(0,0,0)作为分类点
## 方案2：
直接使用affect Representation and Recognition ...论文中的分类标准
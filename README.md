# world-city-observatory

## Introduction

Folder | Content
------------ | -------------
Raw | Data scraped
Data | Data parsed
Images | Graph samples bulit from data

抓取和整理数据的代码在wos.ipynb, 抓取的原始数据在Raw文件夹，整理好的数据在Data文件夹，知识图谱的示例在Images文件夹。
在Data文件夹中，分别提供了以**city**和**urban planning**为搜索关键词的结果，包括过去两周前五十的热词，前十的热门文章和构建知识图谱所需要的矩阵。


## Visualization

对知识图谱进行前端可视化时，可以参考<a href="http://bl.ocks.org/MoritzStefaner/1377729">Force-based label placement</a>的例子。可以看到，在代码中首先定义了`nodes`，然后是`links`。将nodes替换为前五十的keywords，再把矩阵中的数值作为它们之间的连接强度即可实现可视化。矩阵文件中行和列均是按照keywords文件中的顺序，可视化时可以根据连接数值的大小对知识图谱进行简化。



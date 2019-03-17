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

对知识图谱进行前端可视化时，可以参考<a href="https://observablehq.com/@d3/force-directed-graph">Force-Directed Graph</a>的例子。在该例子中，数据存放在<a href="https://observablehq.com/@d3/force-directed-graph">json文件</a>中，对其进行替换即可更新图结构。可以看到，该文件首先定义了nodes，然后是links。将nodes替换为前五十的keywords，再把矩阵中的数值作为它们之间的连接强度即可实现可视化。矩阵文件中行和列均是按照keywords文件中的顺序，可视化时可以根据连接数值的大小对知识图谱进行简化。



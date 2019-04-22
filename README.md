# world-city-observatory

## Introduction

Folder | Content
------------ | -------------
Raw | Data scraped
Data | Data parsed
Images | Graph samples bulit from data

抓取和整理数据的代码在wos.ipynb, 抓取的原始数据在Raw文件夹，整理好的数据在Data文件夹，知识图谱的示例在Images文件夹。
在Data文件夹中，分别提供了以`city`和`urban planning`为搜索关键词的结果，包括过去两周前五十的热词，前十的热门文章、构建知识图谱所需要的矩阵和热词相关文章。


## Visualization

<!-- 对知识图谱进行前端可视化时，可以参考<a href="http://bl.ocks.org/MoritzStefaner/1377729">Force-based label placement</a>的例子。可以看到，在代码中首先定义了`nodes`，然后是`links`。将nodes替换为前五十的keywords，再把矩阵中的数值作为它们之间的连接强度即可实现可视化。矩阵文件中行和列均是按照keywords文件中的顺序，可视化时可以根据连接数值的大小对知识图谱进行简化。
 -->

对知识图谱进行前端可视化时，可以参考<a href="http://bl.ocks.org/paulovn/9686202">The PopCha! Movie Network</a>的例子。可以看到，数据主要存贮在<a href="http://bl.ocks.org/paulovn/raw/9686202/movie-network-25-7-3.json">json文件</a>，在文件中首先定义了`nodes`，然后是`links`。将nodes替换为前五十的keywords，再把矩阵中的数值作为它们之间的连接强度即可实现可视化。node radius取决于热词count，edge width取决于连接值。矩阵文件中行和列均是按照keywords文件中的顺序，可视化时可以根据连接数值的大小对知识图谱进行简化。node moveon时，高亮显示与之相连的nodes，点击时，在侧边栏显示相关的前10篇文章。


## Reference

数据源：
Web of Science https://www.webofknowledge.com/

数据处理：
Anaconda https://www.anaconda.com/ 
Selenium https://www.seleniumhq.org/ 
BeautifulSoup https://www.crummy.com/software/BeautifulSoup/bs4/doc/ 
Networkx https://networkx.github.io/

可视化：
D3 https://d3js.org/ 
Force-based Label Placement http://bl.ocks.org/MoritzStefaner/1377729

代码库：
Github https://github.com/tjciuc/world-city-observatory


#elasticsearchx学习

    一个分布式的实时文档存储，每个字段 可以被索引与搜索
    一个分布式实时分析搜索引擎
    能胜任上百个服务节点的扩展，并支持 PB 级别的结构化或者非结构化数据
     
    免费下载，使用，修改 Elasticsearch。它在 Apache 2 license 协议下发布的， 
    这是众多灵活的开源协议之一。
    Elasticsearch 的源码被托管在 Github 上 github.com/elastic/elasticsearch  

权威指南：
https://www.elastic.co/guide/cn/elasticsearch/guide/current/index.html

Windows安装教程：
https://www.cnblogs.com/hualess/p/11540477.html
下载win版，运行.bat
安装Chrome的elasticsearch插件

5.x,6.x,7.x增删改查语法有版本差异

纵横使用6.x版本，文档：
https://www.elastic.co/guide/en/elasticsearch/reference/6.8/index.html


#RESTFUL API基本类型：

    索引（类似于一个数据库的库名）
    类型（类似于一个数据库中的一张表名）
    文档 (类似于一张表里的一条记录)

基本格式 http://<ip>:<port>/<索引>/<类型>/<文档id>

官方6.x文档操作API:
https://www.elastic.co/guide/en/elasticsearch/reference/6.8/docs.html

es6的字段类型：

https://blog.csdn.net/u014516601/article/details/82885392

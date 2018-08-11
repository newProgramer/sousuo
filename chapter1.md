# 简介

Lucene是简单而功能强大的基于Java的搜索库。它可以用于任何应用程序来搜索功能。 Lucene是开源项目。它是可扩展的，高性能的库用于索引和搜索几乎任何类型的文本。 Lucene库提供了所需的任何搜索应用程序的核心业务。索引和搜索。

![](https://www.yiibai.com/uploads/allimg/141127/11363T304-0.jpg)



### 创建Lucene步骤

1. 创建`Documents`添加`FIelds`
2. 创建一个`IndexWriter`，然后调用`addDocument()`方法添加一个documen
3. 调用`QueryParser.parse()`来构建一个字符串查询
4. 创建一个`IndexSearcher`，然后调用它的`search()`方法




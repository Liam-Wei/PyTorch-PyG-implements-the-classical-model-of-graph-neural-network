![在这里插入图片描述](https://img-blog.csdnimg.cn/b0c2d4ab96584e2bafb2801fee29e3b7.jpeg#pic_center)

# 前言
大家好，我是阿光。

本专栏整理了《图神经网络代码实战》，内包含了不同图神经网络的相关代码实现（PyG以及自实现），理论与实践相结合，如GCN、GAT、GraphSAGE等经典图网络，每一个代码实例都附带有完整的代码。

正在更新中~ ✨  

![在这里插入图片描述](https://img-blog.csdnimg.cn/img_convert/e0fb91ed8ee12ea1d35b3a0339ff9282.jpeg#pic_center)


🚨 我的项目环境：
+ 平台：Windows10
+ 语言环境：python3.7
+ 编译器：PyCharm
+ PyTorch版本：1.11.0
+ PyG版本：2.1.0

---

# 🌠 『精品学习专栏导航帖』

+ **🐧[<font color=Tomato>【Matplotlib绘制图像目录】Python数据可视化之美](https://weibaohang.blog.csdn.net/article/details/128132121)🐧**

+ **🎠[<font color=Sienna>【Pandas数据处理100例目录】Python数据分析玩转Excel表格数据](https://weibaohang.blog.csdn.net/article/details/128067702)🎠**

+ **🐳[<font color=red>最适合入门的100个深度学习实战项目](https://weibaohang.blog.csdn.net/article/details/127365867?spm=1001.2014.3001.5502)🐳**
+ **🐙[<font color=orange>【PyTorch深度学习项目实战100例目录】项目详解 + 数据集 + 完整源码](https://weibaohang.blog.csdn.net/article/details/127128637?spm=1001.2014.3001.5502)🐙**
+ **🐶[<font color=gold>【机器学习入门项目10例目录】项目详解 + 数据集 + 完整源码](https://blog.csdn.net/m0_47256162/article/details/128011714?spm=1001.2014.3001.5501)🐶**
+ **🦜[<font color=green>【机器学习项目实战10例目录】项目详解 + 数据集 + 完整源码](https://blog.csdn.net/m0_47256162/article/details/128055406?spm=1001.2014.3001.5501)🦜**
+ **🐌[<font color=darkcyan>Java经典编程100例](https://blog.csdn.net/m0_47256162/article/details/113728127)🐌**
+ **🦋[<font color=blue>Python经典编程100例](https://blog.csdn.net/m0_47256162/article/details/110746376)🦋**
+ **🦄[<font color=purple>蓝桥杯历届真题题目+解析+代码+答案](https://blog.csdn.net/m0_47256162/article/details/110476937)🦄**
+ **🐯[<font color=deepskyblue>【2023王道数据结构目录】课后算法设计题C、C++代码实现完整版大全](https://weibaohang.blog.csdn.net/article/details/124415748)🐯**

---
对于本专栏的网络模型，分别使用了三种实现方式 `PyG框架实现`、`PyTorch实现`、`Message Passing消息传递机制实现`，小伙伴可以按照自己的能力以及需求学习不同的实现方式。

注意 🚨：本目录中已存在的链接博文已全部写好，例如 ~~+ [（一）：节点分类](https://weibaohang.blog.csdn.net/article/details/128808943)~~ 这类带有删除线的文章表示正在更新中，如果写完会去掉删除线，点击出现404表示文章还没有发布，后续根据情况陆续发布。

### 🌈『目录』 
---
**📢 PyG算子、数据集介绍**

+ [（一）：PyG内置常见图数据集一览表](https://weibaohang.blog.csdn.net/article/details/128808943)
+ [（二）：PyG图神经网络算子一览表](https://weibaohang.blog.csdn.net/article/details/128808649)

---
**📢 图神经网络常见任务与应用场景**

+ [（一）：节点分类（PyG基于GCN实现Cora节点分类任务）](https://weibaohang.blog.csdn.net/article/details/128828619)
+ [（二）：图分类（PyG基于GCN实现MUTAG图分类任务）](https://weibaohang.blog.csdn.net/article/details/128829040)
~~+ [（三）：链路预测](https://weibaohang.blog.csdn.net/article/details/128808649)~~ 
~~+ [（四）：异常检测](https://weibaohang.blog.csdn.net/article/details/128808649)~~ 
~~+ [（五）：社区检测](https://weibaohang.blog.csdn.net/article/details/128808649)~~ 

---
**📢 图嵌入学习（Graph Embedding）**

+ [（一）：DeepWalk（PyG基于DeepWalk实现节点分类及其可视化）](https://weibaohang.blog.csdn.net/article/details/128841614)
+ [（二）：Node2Vec（PyG基于Node2Vec实现节点分类及其可视化）](https://weibaohang.blog.csdn.net/article/details/128840999)
+ [（三）：MetaPath2Vec（PyG基于MetaPath2Vec实现节点分类及其可视化）](https://weibaohang.blog.csdn.net/article/details/128848088)
~~+ [（三）：LINE](https://weibaohang.blog.csdn.net/article/details/128808649)~~ 

---
**📢 图池化（Graph Pooling）**

+ [（一）：EdgePool（Pytorch+PyG实现EdgePool实现图分类）](https://weibaohang.blog.csdn.net/article/details/128858774)
+ [（二）：TopKPool（Pytorch+PyG实现TopKPool实现图分类）](https://weibaohang.blog.csdn.net/article/details/128867064)
+ [（三）：SAGPool（Pytorch+PyG实现SAGPool实现图分类）](https://weibaohang.blog.csdn.net/article/details/128875579)
+ [（四）：ASAPool（Pytorch+PyG实现ASAPool实现图分类）](https://weibaohang.blog.csdn.net/article/details/128892904)

---
**📢 MLP**

+ [（一）：Pytorch+PyG实现MLP(基于PyG实现)](https://weibaohang.blog.csdn.net/article/details/128765310)
+ [（二）：Pytorch实现MLP(基于PyTorch实现)](https://weibaohang.blog.csdn.net/article/details/128809423)

---
**📢 GCN**

+ [（一）：Pytorch+PyG实现GCN(基于PyG实现)](https://weibaohang.blog.csdn.net/article/details/127614247)
+ [（二）：Pytorch实现GCN(基于PyTorch实现)](https://weibaohang.blog.csdn.net/article/details/128739905)
+ [（三）：Pytorch实现GCN(基于Message Passing消息传递机制实现)](https://weibaohang.blog.csdn.net/article/details/128742651)

---
**📢 GAT**

+ [（一）：Pytorch+PyG实现GAT(基于PyG实现)](https://weibaohang.blog.csdn.net/article/details/127583004)
+ [（二）：Pytorch实现GAT(基于PyTorch实现)](https://weibaohang.blog.csdn.net/article/details/128765445)
+ [（三）：Pytorch实现GAT(基于Message Passing消息传递机制实现)](https://weibaohang.blog.csdn.net/article/details/128809998)

---
**📢 GIN**

+ [（一）：Pytorch+PyG实现GIN(基于PyG实现)](https://weibaohang.blog.csdn.net/article/details/128824350)
+ [（二）：Pytorch实现GIN(基于PyTorch实现)](https://weibaohang.blog.csdn.net/article/details/128824153)
+ [（三）：Pytorch实现GIN(基于Message Passing消息传递机制实现)](https://weibaohang.blog.csdn.net/article/details/128823813)

---
**📢 GraphSAGE**

+ [（一）：Pytorch+PyG实现GraphSAGE(基于PyG实现)](https://weibaohang.blog.csdn.net/article/details/128747701)
+ [（二）：Pytorch实现GraphSAGE(基于PyTorch实现)](https://weibaohang.blog.csdn.net/article/details/128820117)
+ [（三）：Pytorch实现GraphSAGE(基于Message Passing消息传递机制实现)](https://weibaohang.blog.csdn.net/article/details/128820531)

---
**📢 EdgeCNN**

+ [（一）：Pytorch+PyG实现EdgeCNN(基于PyG实现)](https://weibaohang.blog.csdn.net/article/details/128767490)
+ [（二）：Pytorch实现EdgeCNN(基于PyTorch实现)](https://weibaohang.blog.csdn.net/article/details/128768970)
+ [（三）：Pytorch实现EdgeCNN(基于Message Passing消息传递机制实现)](https://weibaohang.blog.csdn.net/article/details/128767660)

---
**📢 GraphConv**

+ [（一）：Pytorch+PyG实现GraphConv(基于PyG实现)](https://weibaohang.blog.csdn.net/article/details/128822698)
+ [（二）：Pytorch实现GraphConv(基于PyTorch实现)](https://weibaohang.blog.csdn.net/article/details/128823065)
+ [（三）：Pytorch实现GraphConv(基于Message Passing消息传递机制实现)](https://weibaohang.blog.csdn.net/article/details/128822958)

---

注意🚨：所有文章使用的图数据是经典的 `Cora` 数据集，定义的训练轮数（200轮）以及损失函数优化器都是一致的，由于图网络很容易过拟合导致训练集的分类精度达到 `99.9%`，所以下表中显示的数据都是基于测试集的。

||Accuracy|Loss  |
|--|--|--|
| MLP | 0.1800 | 1.9587 |
| GCN | 0.7200 | 1.3561 |
| GAT | 0.7810 | 1.0362 |
| GIN | 0.7650 | 0.9645 |
| GraphSAGE | 0.7060 | 1.2712 |
| EdgeCNN | 0.3790 | 1.7529 |
| GraphConv | 0.6030 | 1.2378 |

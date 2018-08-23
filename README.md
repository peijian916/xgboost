# xgboost
A very useful machine learning artifact
一、什么是 xgboost？
XGBoost ：eXtreme Gradient Boosting
是由 Tianqi Chen http://homes.cs.washington.edu/~tqchen/ 最初开发的实现可扩展，便携，分布式 gradient boosting (GBDT, GBRT or GBM) 算法的一个库，
可以下载安装并应用于 C++，Python，R，Julia，Java，Scala，Hadoop，现在有很多协作者共同开发维护。XGBoost 所应用的算法就是 gradient boosting decision
tree，既可以用于分类也可以用于回归问题中。

二、为什么要用 xgboost？
XGBoost 就是对 gradient boosting decision tree 的实现，但是一般来说，gradient boosting 的实现是比较慢的，因为每次都要先构造出一个树并添加到整个模型
序列中。而 XGBoost 的特点就是计算速度快，模型表现好，这两点也正是这个项目的目标。

表现快是因为它具有这样的设计：
训练时可以用所有的 CPU 内核来并行化建树。
用分布式计算来训练非常大的模型。
对于非常大的数据集还可以进行 Out-of-Core Computing。
更好地利用硬件。

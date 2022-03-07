
## 简介

AutoML通常通常有两类，一类是Google派，主要是深度学习相关，面向大模型，
面向的数据类型是语音，图像，视频等非结构化的数据类型。
比如说自动寻找最优框架，自动找超参等。

另外就是H2O这种，主要面向BI，更聚焦于传统的机器学习。
主要面向的数据类型是表格类型。

## H2O特性

H2O的AutoML主要做如下工作：
1. data preprocessing: data imputation, one-hot encoding and standardization
2. model generation: automates the process of training and tuning various families of models
   using random grid search.
    Random grid search combined with stacked ensembles is a powerful combination
3. ensembles: H2O AutoML trains two ensembles using stacking. Ensembles perform well if 
   the models they are based on:
   1. are individually strong and 
   2. make uncorrelated errors
   stacking uses a second-level metalearning algorithm to find the optimal combinatin of base learners.


## 资源

一些H2O相关资源：
1. [The different flavors of AutoML](https://www.h2o.ai/blog/the-different-flavors-of-automl/)
2. [Deep Dive Into H2O's AutoML](https://www.h2o.ai/blog/a-deep-dive-into-h2os-automl/)
3. The [slides](https://github.com/business-science/presentations/blob/master/2019_02_13_Learning_Lab_Marketing_Analytics/h2o_automl_bizsci_feb2019.pdf) as part of an insightful presentation on Automatic Machine Learning with H2O AutoML.
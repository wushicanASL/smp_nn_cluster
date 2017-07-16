﻿## smp_nn_cluster

---
* cases.xlsx: 分类的cases输出，可以通过筛选得到bad caese
* smp.tags: 分类标签 + 统计 +　标签对应序号
* smp.pretrain.pkl.gz: 原始句子变为向量后的保存结果，后续直接读取即可
* lstm_smp_31train_31test.py: lstm直接进行分类的代码
* lstm_smp_30train_30test.py: lstm进行分类 但训练集与测试集均除去“未定义”类
* smp_topic_cluster_n.py: 聚类代码 n即聚类中心数目
* lstm_smp_2satge_2-2-30-30.py: 二阶段代码 先分到对应聚类中心 后分小类
* lstm_smp_ntrain_ntest.py: 训练LSTM K+1分类器 n即聚类中心数目
* lstm_smp_2train_2test.py: lstm进行分类 所有“未定义”为一类 所有“已定义”为一类
* 附： ch2r文件夹： ch2r数据集的全部代码

* 待探究： lstm->cnn 
* 待探究： ch2r数据集在 nn_cluster的效果
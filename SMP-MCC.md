# SMP-MCC



## 相关研究

- 相关研究（参考研究综述）
  - Static-RNN，Dynamic-RNN，SI-RNN
  - ICRED，GSN
  - 对话历史的使用



## SMP-MCC 2019

- 解决方案

  - 1st

    - 数据集，针对不同主题，爬取特定主题网站优质数据集
  - 输入，过滤与主题无关的对话历史
    - 模型，BERT预训练词向量，启动句模型（人工构造单轮数据集，Seq2Seq + Attention） + 生成式模型（BiLSTM + Attention） + 检索式模型（群聊对话历史 + BM25） + 全局策略（规则关键词匹配）

    <img src="/Users/kaiyan/Library/Application Support/typora-user-images/image-20200702123312727.png" alt="image-20200702123312727" style="zoom: 33%;" />
  
  - 2nd
  
    GPT，百度知道数据集



## SMP-MCC 2020

总体延续 SMP-MCC 2019 设定，提供数据集和工具包参考，以及在线自动评测网站和排行榜等。



- 数据集介绍

  豆瓣小组爬去，进行数据清洗，数据规模

- baseline介绍

  - GPT生成式
  - 检索式，BM25算法

- 当前榜单情况
# Dialogue Challenge Tutorial

> 人机对话相关评测总结（侧重SMP中文人机对话评测介绍，[对话评测组织及经验分享](对话评测组织及经验分享.pdf)）

[TOC]

|              | DSTC                                                         | ConvAI                   | SMP-ECDT                                                 | JD DC              | SMP-MCC        |
| ------------ | ------------------------------------------------------------ | ------------------------ | -------------------------------------------------------- | ------------------ | -------------- |
| **组织机构** | MSR/Alexa/CMU<br>Facebook/IBM/Google                         | DeepPavlov               | 哈工大<br>科大讯飞<br>清华大学                           | 京东/智源          | 哈工大         |
| **任务简述** | 端到端任务型对话<br>回复生成/检索等<br>基于知识的对话<br>多模态对话 | 个性化对话<br>开放域对话 | 意图分类<br>任务型对话<br>小样本语言理解<br>知识驱动对话 | 客服对话<br>多模态 | 机器人群聊对话 |
| **评测方式** | 客观+人工                                                    | 客观+人工                | 客观+人工                                                | 客观+人工          | 客观+人工      |
| **评测时间** | 2012-2020                                                    | 2017-2020                | 2017-2020                                                | 2018/2020          | 2019/2020      |



## SMP-ECDT

> 由哈工大、科大讯飞和清华大学联合承办的中文人机对话评测
>
> 相关解决方案见 SMP-ECDT 2017/18/19 文件夹

- [SMP-ECDT 2017](http://ir.hit.edu.cn/smp2017-ecdt) , [评测数据](https://github.com/HITlilingzhi/SMP2017ECDT-DATA)
  - 任务1：用户意图领域分类
  - 任务2：特定域任务型人机对话在线评测

- [SMP-ECDT 2018](https://www.steamedfish.cn/2018/09/30/%E3%80%90%E7%B2%BE%E5%BD%A9%E7%BB%A7%E7%BB%AD%E3%80%91SMP2018%E4%B8%AD%E6%96%87%E4%BA%BA%E6%9C%BA%E5%AF%B9%E8%AF%9D%E6%8A%80%E6%9C%AF%E8%AF%84%E6%B5%8B%EF%BC%88ECDT%EF%BC%89%E5%88%B7%E6%A6%9C%E5%85%AC%E5%91%8A/)
  - 任务1：用户意图领域分类
  - 任务2：特定域任务型人机对话在线评测
  - 相关参考
    - [SMP2018中文人机对话技术评测 论文摘要](https://www.jiqizhixin.com/articles/2019-03-06-13)

    - [SMP-ECDT 2018评测总结](https://mp.weixin.qq.com/s/_VHEuXzR7oXRTo5loqJp8A)
    - [深思考第一名方案](https://www.jiqizhixin.com/articles/080601)
    - [桔子互动方案](https://zhuanlan.zhihu.com/p/43419905)

- [SMP-ECDT 2019](http://conference.cipsc.org.cn/smp2019/evaluation.html), [排行榜](https://adamszq.github.io/smp2019ecdt_task1/)
  - 任务1：自然语言理解评测
  - 任务2：个性化对话竞赛

- [SMP-ECDT 2020](https://smp2020.aconf.cn/smp.html#3)
  - 任务1：小样本对话语言理解技术评测
  - 任务2：知识驱动的多轮对话竞赛
  - [参赛队伍评测报告视频, 提取码: ijcw](https://pan.baidu.com/s/1TmzQ3VYJQsOzlP17-nGJVw)



## SMP-MCC

> 主要由哈工大承办的机器人群聊比赛
>
> 相关解决方案见 SMP-MCC 2019 文件夹

- [SMP-MCC 2019](http://ir.hit.edu.cn/smp-mcc)

- [SMP-MCC 2020](http://mcc.8wss.com/)



## JDDC

> 由京东和智源组织的关于客服对话和多模态对话的评测

- [JDDC 2019](https://jddc.jd.com/2019/)

- [JDDC 2020](https://jddc.jd.com/), [CCL 2020](http://www.cips-cl.org/static/CCL2020/evaluationtasks.html)



## CCL中移在线

> 中移在线客服领域用户意图分类

[CCL 2018](http://www.cips-cl.org/static/CCL2018/call-evaluation.html), [冠军方案](https://github.com/nlpjoe/2018-CCL-UIIMCS)



## DSTC

> Dialog System Technology Challenge (DSTC)
>
> 2012-2020，每年由高校或企业机构发布多项对话任务，包括任务型和多模态对话等等

- [DSTC1](https://www.microsoft.com/en-us/research/event/dialog-state-tracking-challenge/#!dstc1-information), [DSTC2/3](http://camdial.org/~mh521/dstc/), [DSTC4](http://www.colips.org/workshop/dstc4/), [DSTC5](http://workshop.colips.org/dstc5/tasks.html)

- [DSTC6](http://workshop.colips.org/dstc6)
  - Track1 End-to-End Goal Oriented Dialog Learning
  - Track2 End-to-End Conversation Modeling
  - Track3 Dialogue Breakdown Detection

- [DSTC7](http://workshop.colips.org/dstc7/call.html)
  - Track1 Sentence Selection
  - Track2 Sentence Generation
  - Track3  Audio Visual Scene-aware dialog (AVSD)

- [DSTC8](https://sites.google.com/dstc.community/dstc8/tracks)
  - Track1 [Multi-domain Task Completion](https://www.microsoft.com/en-us/research/project/multi-domain-task-completion-dialog-challenge/)
  - Track2 [NOESIS II: Predicting Responses](https://github.com/dstc8-track2/NOESIS-II/)
  - Track3 [Audio Visual Scene-Aware Dialog](https://github.com/dialogtekgeek/DSTC8-AVSD)
  - Track4 [Schema-Guided State Tracking](https://github.com/google-research-datasets/dstc8-schema-guided-dialogue)

- [DSTC9](https://sites.google.com/dstc.community/dstc9/tracks)
  - Track1 [Beyond Domain APIs: Task-oriented Conversational Modeling with Unstructured Knowledge Access](https://github.com/alexa/alexa-with-dstc9-track1-dataset)
  - Track2 [Multi-domain Task-oriented Dialog Challenge II](https://www.microsoft.com/en-us/research/project/multi-domain-task-completion-dialog-challenge-ii/)
  - Track3 [Interactive Evaluation of Dialog](http://dialog.speech.cs.cmu.edu:8003/)
  - Track4 [SIMMC: Situated Interactive Multi-Modal Conversation AI](https://github.com/facebookresearch/simmc)



## ConvAI

> [DeepPavlov/convai](https://github.com/DeepPavlov/convai)

- [ConvAI1](https://github.com/DeepPavlov/convai/tree/master/2017)
  - Teams are expected to submit dialogue systems able to carry out intelligent and natural conversations about specific news articles with humans
- [ConvAI2](https://github.com/DeepPavlov/convai/tree/master/2018)
  - [The Persona-Chat task](http://convai.io/#personachat-convai2-dataset)
- [ConvAI3](https://github.com/DeepPavlov/convai)
  - a user is asking an ambiguous question (a question to which one can return > 1 possible answers);
  - the system must identify that the question is ambiguous, and, instead of trying to answer it directly, ask a good clarifying question.



## AIWolfDial

> 组织机器人进行狼人杀游戏

[official website](http://aiwolf.org/en/)

[1st International AI Competition on Werewolf Game](http://aiwolf.org/en/archives/2023)

[2nd International Aiwolf Contest](http://aiwolf.org/en/2nd-international-aiwolf-contest)

[AIWolf platform](http://aiwolf.org/en/server)

[AIWolfDial2019](https://aiwolfdial.kanolab.net/)



## GLUE/SuperGLUE

> The General Language Understanding Evaluation (GLUE)

[GLUE](https://gluebenchmark.com/), [SuperGLUE](https://super.gluebenchmark.com/)


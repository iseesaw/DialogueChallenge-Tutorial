# SMP-ECDT



## SMP-ECDT 2017

[SMP-ECDT 2017](http://ir.hit.edu.cn/smp2017-ecdt)，[评测数据](https://github.com/HITlilingzhi/SMP2017ECDT-DATA)

[第一名华南农业大学方案](https://blog.csdn.net/c9Yv2cf9I06K2A9E/article/details/78141022?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-3.nonecase&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-3.nonecase)

### 任务1：用户意图领域分类

在人机对话系统地应用过程中，用户可能会有多种意图，相应地会触发人机对话系统中的多个领域，其中包括任务型垂直领域（如查询机票、酒店、公交车等）、知识型问答以及闲聊等。因而，人机对话系统地一个关键任务就是正确地将用户的输入分类到相应地领域中，从而才能返回正确的回复结果。

- 评测说明

  评测任务中包含闲聊和垂类两大类，其中垂类又细分为30个垂直领域。本次评测任务中，仅考虑针对单对话轮用户意图的领域分类，多轮对话整体意图的领域分类不在此评测范围之内。

- 评测方式

  分为封闭式评测（仅允许使用主办方提供的评测数据进行训练和开发）和开放式评测（可以开放地获取除主办方提供的数据之外的训练及开发数据）

- 评价指标

  准确率、召回率和F值

- 数据示例

  ![image-20200629133800862](/Users/kaiyan/Library/Application Support/typora-user-images/image-20200629133800862.png)

- 系统提交及测试

  参赛者提交最终系统，组委会在封闭测试集上验证结果。

  参评者自行根据组织方提供的服务端模版修改并搭建服务，评测当日，组织方批量向所有参评者同时发送请求，内含测试服务能够正常运行的用例和正式评测用例，获取分类结果并记录。

- 解决方案

  TODO



### 任务2：特定域任务型人机对话在线评测

- 评测说明

  本次评测任务2的特定领域包括：机票类、火车票类和酒店类3个垂直领域，系统通过与测试人员实时在线对话完成相应的预定或查询任务，满足测试人员的需求。

- 评测方式

  任务2采用人工评价的方式，对于每个参赛系统，主办方提供给测试人员完整的用户意图描述，对于任意相同的用户意图描述，对不同的参赛系统均给定相同的首轮对话输入，启动在线评测，评测过程中评测员根据给定的完整意图描述与参赛系统进行交互，直至对话结束。对话结束的条件为系统返回所有任务（单任务或多任务）的执行结果（出于对模拟终端设备显示区域大小限制的考虑，单任务的多条结果只显示相关性最高的前5条），或超过50个对话轮数之后仍未返回测试员所需的结果，测试员手动结束对话测试。

- 评价指标

  - 任务完成率

  - 用户满意度

  - 回复语言的自然度

  - 对话轮数

  - 静态的数据库资源未覆盖情况的引导能力

    举例来说，如果当前只支持查询十日航班，那么当查到十日之外信息时，是否能友好的引导。

  > 注：除“对话轮数”之外，以上指标均由人工给出评分。

- 数据示例

  - 完整的用户意图描述示例
  - Json格式的静态航班、酒店、火车票数据资源
  - 人工对话示例

  <img src="/Users/kaiyan/Library/Application Support/typora-user-images/image-20200629134654912.png" alt="image-20200629134654912" style="zoom:50%;" />

- 在线测试及结果评价

  参赛系统以Web Service的形式提供系统调用，测试人员在线进行特定域任务型人机对话测试，并在测试后进行结果评价。

- 解决方案

  TODO



## SMP-ECDT 2018

[SMP-ECDT 2018](https://www.steamedfish.cn/2018/09/30/%E3%80%90%E7%B2%BE%E5%BD%A9%E7%BB%A7%E7%BB%AD%E3%80%91SMP2018%E4%B8%AD%E6%96%87%E4%BA%BA%E6%9C%BA%E5%AF%B9%E8%AF%9D%E6%8A%80%E6%9C%AF%E8%AF%84%E6%B5%8B%EF%BC%88ECDT%EF%BC%89%E5%88%B7%E6%A6%9C%E5%85%AC%E5%91%8A/)

[SMP2018中文人机对话技术评测 论文摘要](https://www.jiqizhixin.com/articles/2019-03-06-13)

[SMP-ECDT 2018评测总结](https://mp.weixin.qq.com/s/_VHEuXzR7oXRTo5loqJp8A)

[深思考第一名方案](https://www.jiqizhixin.com/articles/080601)

[桔子互动方案](https://zhuanlan.zhihu.com/p/43419905)

相比于上一届的区别：

- 我们分别为两个任务加入了新的数据集，新加入的数据集都是由专业数据标注人员标注的，并且我们在测试集中加入了大量的干扰数据用于保证评测数据的隐蔽性。
- 本次评测任务一取消了封闭域的评测，只进行开放域评测，区别是用户不仅可以使用我们提供的训练数据，还可以自行收集数据。
- 我们在任务二的评价指标上做出了优化，更新了未完成任务对话轮数的计算方式，从而使统计出的平均对话轮数更加合理。



### 任务1：用户意图领域分类

包含闲聊和垂类两大类，其中垂类又细分为30个垂直领域，参赛系统需要判定用户的输入所属的类别。

- 评测说明

  刷榜评测数据标签包含闲聊和垂类两大类，其中垂类又细分为30个垂直领域，评测数据共计31个类别。本次评测任务中，仅考虑针对单轮对话用户意图的领域分类，多轮对话整体意图的领域分类不在此次评测范围之内。

- 评测方式

  为了保证比赛的公平性和刷榜评测的可操作性，本次评测中使用CodaLab在线评测平台，并将评测的相关数据放在了此平台上。

- 评价指标

  精准率、召回率及F值

- 数据示例

  ![image-20200629190740525](/Users/kaiyan/Library/Application Support/typora-user-images/image-20200629190740525.png)



### 任务2：特定域任务型人机对话在线评测

参赛系统通过与测试人员实时在线对话完成相应的预定或查询任务，完成测试人员的特定域需求。

- 具体描述为：对于一个查询并预定机票、火车票或酒店的一个或多个意图的混合任务，根据给定的数据库数据构建系统引导用户完成相应的任务。本次评测仍采用人工在线评测的方法，一个完整意图描述为：“预定明天从北京去上海的上午或者中午出发的机票”，其订机票过程如表2所示：

- 评价指标

  为了保证任务型对话系统各个方面的主观和客观性能，本次评测采用了以下指标：

  - 任务完成率：每个测试对话看作是一个任务，测试过程中完成的任务数占任务总数的比率。
  - 平均对话轮数：完成一个任务所产生的对话句子数，在完成任务的前提下越少越好。
  - 用户满意度：评测员对系统的客观打分，包含5个取值{-2, -1, 0, 1, 2}
  - 回复流畅度：主观打分，包含3个取值{-1, 0, 1}
  - 未覆盖数据引导能力：主观打分，包含2个取值{0, 1}

- 数据说明

  任务二的数据库数据仍来自科大讯飞股份有限公司，该数据集包括自系统日期起一个月的机票、火车票以及各地酒店信息，此外，我们人工写了若干个测试任务，包含订机票、订火车票、订宾馆三种简单意图任务或多意图任务。
  
  | Agent | Response                                                     |
  | ----- | ------------------------------------------------------------ |
  | User  | 查询明天从北京去上海的机票                                   |
  | Robot | 请问您需要订票吗？                                           |
  | User  | 是的                                                         |
  | Robot | 请问您要明天什么时候出发呢？                                 |
  | User  | 上午或中午吧                                                 |
  | Robot | 帮您查询了明天从北京到上海的机票，没有上午出发的航班，中午12:10出发是否可以？7.3折，910元 |
  | User  | 也行，就订这个吧                                             |
  | Robot | 已经帮您预订该航班机票，将跳转至付款页面                     |



## SMP-ECDT 2019

[SMP-ECDT 2019](http://conference.cipsc.org.cn/smp2019/evaluation.html)



### 任务1：自然语言理解评测

- 任务描述

  本次评测包括领域分类、意图识别和语义槽填充三项子任务，例如给定一个用户的表达句子“我想订上海飞往北京的航班”，则该句的：

  - 领域为：“机票”
  - 意图为：“订机票”
  - 语义槽为：
    - departCity：上海
    - arriveCity：北京

- 评测说明

  本次评测包括单轮对话用户意图的领域分类、意图识别和语义槽填充任务，多轮对话整体意图的理解不在此次评测范围之内。

- 评测方式

  参赛者报名后，可以获取主办方提供的评测数据（包括训练及开发数据）。评测时，参赛者在线提交评测系统（Codalab），主办方在测试集上运行评测系统并得出评测结果，参赛者可以多次提交评测系统，评测结果实时更新并公开排名。

- 评测指标

  对于领域分类、意图识别，我们采用准确率（acc）来评价。

  对于语义槽填充，我们采用F值来评价。

  对于domain，当预测的值与标准答案相同时即为正确。

  对于intent来说，当domain预测正确，且intent的预测的值与标准答案相同时才为正确。

  对于slots来说，我们采用F值作为评价指标，当预测的slots的一个key-value组合都符合标准答案的一个key-value组合才为正确(domain和intent的也必须正确)。

  为了综合考虑模型的能力，我们最终采用句准确率（sentence acc）来衡量一句话领域分类、意图识别和语义槽填充的综合能力，即以上三项结果全部正确时候才算正确，其余均算错误。**本次评测最终以sentence** **acc作为最后评价指标。**



### 任务2：个性化对话竞赛

略……（皓宇师兄介绍ConvAI2）

在对话场景下，已知对话上下文和所有对话参与者的个性化属性，要求生成符合给定个性化特征与上下文逻辑的回复R。

所谓个性化属性由一系列键值对（如<性别，男>，<年龄，90后>）描述：
$$
S=<k_1, v_1>, <k_2, v_2>, \cdots, <k_n ,v_n>
$$
所生成的回复R需要足够流畅、与对话上下文语义相关并且符合所指定的发话人个性化特征。



## SMP-ECDT 2020

[SMP-ECDT 2020](https://smp2020.aconf.cn/smp.html#3)



### 任务1：小样本对话语言理解技术评测

对话语言理解SLU（Spoken Language Understanding）是任务型对话系统的关键组合模块，它把用户的自然语言输入（Utterance）转化为结构化信息（Semantic Frame）以为后续的对话状态管理和回复生成提供支持。其中 Semantic Frame 包括用户意图（Intent）和语义槽（Slot）。

区别于普通的对话语言理解，本评测关注小样本学习场景，即每个测试类别只有几个标注样例。具体任务如图三所示，模型先在一些数据充足的领域训练，然后在未见的新领域上测试。针对一个领域，我们每次给定模型一个带标注的支撑样本集（Support Set）作为参考，让模型对任意未见过的查询样本集（Query Set）标注用户意图和槽位。以图中测试领域为例，给定Support Set，和Query句“播放阿凡达”，模型需要预测出意图为“播放电影”，槽位为【电影：阿凡达】。（通常训练时为模拟小样本情形，训练领域数据也会构造为Support-Query形式训练模型，这里不做强制要求）

![](https://file.aconf.org/conf/hz/2020/03/174917/images/007S8ZIlly1gehkxmifxkj319g0gsk3n.jpg)



### 任务2：知识驱动的多轮对话竞赛

在对话场景下，已知对话上下文和所有知识图谱信息，要求生成符合知识图谱信息与上下文逻辑的对话回复。

知识图谱由一系列三元组（如<头实体，关系，尾实体>）描述。

所生成的对话回复需要足够流畅、与对话上下文语义相关并且符合相关的知识图谱信息。
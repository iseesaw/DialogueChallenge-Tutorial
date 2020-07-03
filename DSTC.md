# DSTC

> Dialog System Technology Challenge (DSTC)



## Introduce

[多轮对话状态追踪（DST）--模型介绍篇](https://zhuanlan.zhihu.com/p/40988001)

[Review on Intent Classification and Slot Filling](https://sara-hy.github.io/2018/11/02/intent_slot/)

任务型对话，自然语言理解，包括意图识别和槽位填充



## DSTC1

[DSTC1](https://www.microsoft.com/en-us/research/event/dialog-state-tracking-challenge/#!dstc1-information)

DSTC1 used human-computer dialogs in the bus timetable domain.



> 公交线路查询，目标固定不变。共5个slot（路线，出发点，终点，日期，时间）
>
> 用户的目标在对话过程中不会发生变化
>
> 最好方案使用判别+生成+无监督自适应，NN方法效果一般，不如人工规则



## DSTC2 & DSTC3

[DSTC2/3](http://camdial.org/~mh521/dstc/)

DSTC2/3 used human-computer dialogs in the restaurant information domain.



> 餐馆预订，用户查询满足特定条件下的餐馆的某些信息（电话、地址等）
>
> 用户目标在对话过程中发生变化
>
> 大部分队伍开始尝试使用NN的方法，大多尝试序列建模（CRF，HMM）
>
> web ranking 的效果也比较好，很多队伍直接使用 ARS 结果，不再使用 SLU 组件



## DSTC4

[DSTC4](http://www.colips.org/workshop/dstc4/)

DSTC4 used human-human dialogs in the tourist information domain.



## DSTC5

[DSTC5](http://workshop.colips.org/dstc5/tasks.html)

DSTC5 used human-human dialogs in the tourist information domain, where training dialogs were provided in one language, and test dialogs were in a different language.



## DSTC6

[DSTC6](http://workshop.colips.org/dstc6)

### Track1 End-to-End Goal Oriented Dialog Learning

This task is aiming to build End-toEnd dialog systems for goal-oriented applications.



### Track2 End-to-End Conversation Modeling

The target of the track is to generate responses of dialog systems automatically using End-to-End training of neural networks using Human-to-Human dialog corpus.



### Track3 Dialogue Breakdown Detection

The track is aiming to detect whether the system utterance causes dialogue breakdown indicating a situation in a dialog where users cannot proceed with the conversation in a given dialog context.



## DSTC7

[DSTC7](http://workshop.colips.org/dstc7/call.html)

### Track1 Sentence Selection

The goal of the system is that given a partial conversation, select the correct next utterances from a set of candidates' and even indicate that none of the proposed utterances is a good candidate.



### Track2 Sentence Generation

The goal is to generate conversational responses that go beyond chitchat, by injecting informational responses that are grounded in external knowledge(e.g., Foursquare, or possibly also Wikipedia, Goodreads, or TripAdvisor).



### Track3  Audio Visual Scene-aware dialog (AVSD)

The task is aiming to generate system responses in a dialog about an input video.

Audio Visual Scene-aware dialog systems could be developed by integrating state-of-the-art technologies from multiple research areas, including: 

- end-to-end dialog technologies, which generate system responses using models trained from dialog data; 
- visual question answering(VQA) technologies, which answer to question aobut images using learned image features; 
- video description technologies, in which videos are described/narrated using multimodal information.



## DSTC8

[DSTC8](https://sites.google.com/dstc.community/dstc8/tracks)

### Track1 [Multi-domain Task Completion](https://www.microsoft.com/en-us/research/project/multi-domain-task-completion-dialog-challenge/)

This challenge proposal intends to foster progress in two important aspects of dialog    systems: dialog complexity and scaling to new domains.

- End-to-end Multi-domain Task

  To advance state-of-the-art technologies for handling complex dialogs, we offer a timely task focusing on multi-domain end-to-end task completion dialog.



- Fast Adaptation Task

  The goal of Task 2 is to investigate whether a dialog system that was trained on a large corpus can learn to converse about a new domain given a much smaller in-domain corpus.



### Track2 [NOESIS II: Predicting Responses](https://github.com/dstc8-track2/NOESIS-II/)

[Task Proposal](https://drive.google.com/file/d/1rCCRsuZ7rq2KGEnT-pBCF6WS47yEsIJA/view)

对 DSTC7 Track1(NOESIS: Noetic End-to-End Response Selection Challenge) 拓展



### Track3 [Audio Visual Scene-Aware Dialog](https://github.com/dialogtekgeek/DSTC8-AVSD)

[Task Proposal](https://drive.google.com/file/d/12h9M7zn-o7jtmHHqHQem66i2UEtS85Op/view)

The task is to build a system that generates responses in a dialog about an input video.

- Task1: Video and Text
- Task2: Text Only



### Track4 [Schema-Guided State Tracking](https://github.com/google-research-datasets/dstc8-schema-guided-dialogue)

These conversations involve interactions with services and APIs spanning 20 domains, ranging from banks and events to media, calendar, travel, and weather.

The wide range of available annotations can be used for intent prediction, slot filling, dialogue state tracking, policy imitation learning, language generation, user simulation learning, among other tasks in large-scale virtual assistants.

Besides these, the dataset has unseen domains and services in the evaluation set to quantify the performance in zero-shot or few shot settings.



## DSTC9

[DSTC9](https://sites.google.com/dstc.community/dstc9/tracks)

### Track1 [Beyond Domain APIs: Task-oriented Conversational Modeling with Unstructured Knowledge Access](https://github.com/alexa/alexa-with-dstc9-track1-dataset)

Track participants will develop dialogues systems to understand relevant domain knowledge, and generate system responses with the relevant selected knowledge.



### Track2 [Multi-domain Task-oriented Dialog Challenge II](https://www.microsoft.com/en-us/research/project/multi-domain-task-completion-dialog-challenge-ii/)

- End-to-end Multi-domain Task Completion Dialog

  In this task, participants will develop an end-to-end dialog system that receives natural language as an input and generates natural language as an output in the travel planning setting.

  The system will be evaluated in MultiWOZ 2.1 dataset setting with ConvLab-2.



- Cross-lingual Multi-domain Dialog State Tracking

  To advance state-of-the-art technologies in handling cross-lingual multi-domain dialogs, we offer the task of building cross-lingual dialog state trackers with a training set in resource-rich language, and dev/test set in a resource-poor language.

  In particular, this task consists of two sub-tasks. One uses English as the resource-rich language and Chinese as the resource-poor language on the MultiWOZ dataset, and the other one uses Chinese as the resource-rich language and English as the resource-poor language on the CrossWOZ dataset.



### Track3 [Interactive Evaluation of Dialog](http://dialog.speech.cs.cmu.edu:8003/)

This track is intended to move research beyond datasets, and evaluate models in interactive environments with real.

- Task1: Static Evaluation of Dialog

  Build better models for dialog response generation

- Task2: Interactive Evaluation of Dialog

  Build/adapt conversation models to work effectively in an interactive setting



### Track4 [SIMMC: Situated Interactive Multi-Modal Conversation AI](https://github.com/facebookresearch/simmc)

The SIMMC challenge aims to lay the foundations for the real-world assistant agents that can handle multimodal inputs, and perform multimodal actions.


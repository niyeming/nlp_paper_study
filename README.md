# 【关于 NLP】 那些你不知道的事

> 作者：杨夕
> 
> 项目地址：https://github.com/km1994/nlp_paper_study
> 
> 个人介绍：大佬们好，我叫杨夕，该项目主要是本人在研读顶会论文和复现经典论文过程中，所见、所思、所想、所闻，可能存在一些理解错误，希望大佬们多多指正。
> 
> NLP 面经地址：https://github.com/km1994/NLP-Interview-Notes

![](other_study/resource/pic/微信截图_20210301212242.png)

> NLP && 推荐学习群【人数满了，加微信 blqkm601 】

![](other_study/resource/pic/20210523220743.png)


- [【关于 NLP】 那些你不知道的事](#关于-nlp-那些你不知道的事)
  - [介绍](#介绍)
    - [【关于 论文工具】那些你不知道的事](#关于-论文工具那些你不知道的事)
    - [NLP 学习篇](#nlp-学习篇)
      - [经典会议论文研读篇](#经典会议论文研读篇)
      - [理论学习篇](#理论学习篇)
        - [经典论文研读篇](#经典论文研读篇)
        - [【关于 transformer 】 那些的你不知道的事](#关于-transformer--那些的你不知道的事)
        - [【关于 Dropout】 那些你不知道的事](#关于-dropout-那些你不知道的事)
        - [【关于 预训练模型】 那些的你不知道的事](#关于-预训练模型-那些的你不知道的事)
        - [【关于 信息抽取】 那些的你不知道的事](#关于-信息抽取-那些的你不知道的事)
          - [【关于 实体关系联合抽取】 那些的你不知道的事](#关于-实体关系联合抽取-那些的你不知道的事)
          - [【关于 命名实体识别】那些你不知道的事](#关于-命名实体识别那些你不知道的事)
          - [【关于 关系抽取】那些你不知道的事](#关于-关系抽取那些你不知道的事)
          - [【关于 文档级别关系抽取】那些你不知道的事](#关于-文档级别关系抽取那些你不知道的事)
          - [【关于 事件抽取】那些你不知道的事](#关于-事件抽取那些你不知道的事)
        - [【关于 知识图谱 】 那些的你不知道的事](#关于-知识图谱--那些的你不知道的事)
          - [【关于 实体链指篇】 那些的你不知道的事](#关于-实体链指篇-那些的你不知道的事)
          - [【关于 实体消歧 】 那些的你不知道的事](#关于-实体消歧--那些的你不知道的事)
          - [【关于KGQA 】 那些的你不知道的事](#关于kgqa--那些的你不知道的事)
          - [【关于Neo4j  】 那些的你不知道的事](#关于neo4j---那些的你不知道的事)
        - [【关于 细粒度情感分析】 那些的你不知道的事](#关于-细粒度情感分析-那些的你不知道的事)
        - [【关于 主动学习】 那些的你不知道的事](#关于-主动学习-那些的你不知道的事)
        - [【关于 对抗训练】 那些的你不知道的事](#关于-对抗训练-那些的你不知道的事)
        - [【关于 GCN in NLP 】那些你不知道的事](#关于-gcn-in-nlp-那些你不知道的事)
        - [【关于 文本预处理】 那些的你不知道的事](#关于-文本预处理-那些的你不知道的事)
        - [【关于问答系统】 那些的你不知道的事](#关于问答系统-那些的你不知道的事)
        - [【关于 文本摘要】 那些的你不知道的事](#关于-文本摘要-那些的你不知道的事)
        - [【关于 文本匹配】 那些的你不知道的事](#关于-文本匹配-那些的你不知道的事)
        - [【关于 机器翻译】 那些的你不知道的事](#关于-机器翻译-那些的你不知道的事)
        - [【关于 文本生成】 那些的你不知道的事](#关于-文本生成-那些的你不知道的事)
        - [【关于 对话系统】 那些的你不知道的事](#关于-对话系统-那些的你不知道的事)
          - [【关于 自然语言生成NLG 】那些你不知道的事](#关于-自然语言生成nlg-那些你不知道的事)
          - [【关于 E2E 】那些你不知道的事](#关于-e2e-那些你不知道的事)
        - [【关于 Rasa 】 那些的你不知道的事](#关于-rasa--那些的你不知道的事)
        - [【关于 半监督学习】 那些的你不知道的事](#关于-半监督学习-那些的你不知道的事)
        - [【关于 NLP分类任务】那些你不知道的事](#关于-nlp分类任务那些你不知道的事)
        - [【关于 中文分词】那些你不知道的事](#关于-中文分词那些你不知道的事)
        - [【关于 关键词提取】 那些你不知道的事](#关于-关键词提取-那些你不知道的事)
        - [【关于 搜索引擎】 那些你不知道的事](#关于-搜索引擎-那些你不知道的事)
        - [【关于 文本纠错】 那些你不知道的事](#关于-文本纠错-那些你不知道的事)
      - [实战篇](#实战篇)
        - [重点推荐篇](#重点推荐篇)
    - [会议收集篇](#会议收集篇)
    - [Elastrsearch 学习篇](#elastrsearch-学习篇)
    - [竞赛篇](#竞赛篇)
      - [【关于 NLP比赛】 那些你不知道的事](#关于-nlp比赛-那些你不知道的事)
      - [【关于 NLP 比赛方案学习】 那些你不知道的事](#关于-nlp-比赛方案学习-那些你不知道的事)
        - [【关于 NLP 比赛方案学习】 那些你不知道的事](#关于-nlp-比赛方案学习-那些你不知道的事-1)
    - [学习资源](#学习资源)
    - [NLP 数据集](#nlp-数据集)
    - [GCN_study学习篇](#gcn_study学习篇)
  - [参考资料](#参考资料)

## 介绍

### [【关于 论文工具】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/other_study/论文学习idea/)

- 问题
  - 作为一名 scholar，你是否和我一样，在刚入门 NLP 时，对于陌生领域有种无从下手，心存畏惧？
  - 作为一名 scholar，你是否还在发愁如何找好的论文？
  - 作为一名 scholar，你是否还在为 自己 的 英文阅读 能力跟不上 很烦恼？
  - 作为一名 scholar，你是否还在为 看到 一篇好paper，但是复现不出 code 而心累？
  - 作为一名 scholar，你是否还在为 有Good idea，Outstanding Experimental results，Beautiful Chinese manuscript，结果 Bad English manuscript, Poor Journal 而奔溃？
  - 作为一名 scholar，你是否在为搞科研没人交流而自闭？
- 当你看到这一篇文档，你将不在为这些问题而烦恼，因为我们为你准备了一整套免费的从 论文查找->论文翻译->论文理解->相关代码搜索->写英文稿->科研学术交流 的路径。
  - [论文不会找怎么办？](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#论文不会找怎么办)
    - [顶会资讯](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#顶会资讯)
    - [论文搜索和分析工具](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#论文搜索和分析工具)
  - [外文读不懂怎么办？](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#外文读不懂怎么办)
    - [论文翻译神器 ———— 通天塔](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#论文翻译神器--通天塔)
    - [论文翻译小助手 ———— 彩云小译](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#论文翻译小助手--彩云小译)
  - [外文没 code 怎么办？](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#外文没-code-怎么办)
    - [papers with code](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#papers-with-code) 
    - [OpenGitHub 新项目快报](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#opengithub-新项目快报) 
  - [外文写起来麻烦怎么办](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#外文写起来麻烦怎么办) 
    - [Overleaf](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#overleaf) 
    - [Authorea](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#authorea) 
    - [Code ocean](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#code-ocean) 
  - [搞科研没人交流怎么办？](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#搞科研没人交流怎么办) 
    - [Shortscience](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#shortscience) 
    - [OpenReview](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#openreview) 
    - [Scirate](https://github.com/km1994/nlp_paper_study/tree/master/论文学习idea#scirate) 


### NLP 学习篇

#### 经典会议论文研读篇

- [ACL2020](ACL/ACL2020.md)
  - [【关于 CHECKLIST】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/other_study/meeting/ACL_study/ACL2020_bertpaper_CHECKLIST/)
    - 阅读理由：ACL2020 best paper ，利用 软件工程 的 思想 思考 深度学习
    - 动机：针对 train-val-test 分割方法 评估 模型性能容易出现 不全面、偏向性、可解性差问题；
    - 方法：提出了一种模型无关和任务无关的测试方法checklist，它使用三种不同的测试类型来测试模型的独立性。
    - 效果：checklist揭示了大型软件公司开发的商业系统中的关键缺陷，表明它是对当前实践的补充好吧。测试使用 checklist 创建的模型可以应用于任何模型，这样就可以很容易地将其纳入当前的基准测试或评估中管道。

#### 理论学习篇

##### 经典论文研读篇

- 那些你所不知道的事
  - [【关于Transformer】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/transformer_study/Transformer/)
  - [【关于Bert】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/T1_bert/)

##### 【关于 transformer 】 那些的你不知道的事

- [【关于Transformer】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/)  transformer 论文学习
  - [【关于Transformer】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/Transformer/)
    1. 为什么要有 Transformer?
    2. Transformer 作用是什么？
    3. Transformer 整体结构怎么样？
    4. Transformer-encoder 结构怎么样？
    5. Transformer-decoder 结构怎么样?
    6. 传统 attention 是什么?
    7. self-attention 长怎么样?
    8. self-attention 如何解决长距离依赖问题？
    9. self-attention 如何并行化？
    10. multi-head attention 怎么解?
    11. 为什么要 加入 position embedding ？
    12. 为什么要 加入 残差模块？
    13. Layer normalization。Normalization 是什么?
    14. 什么是 Mask？
    15. Transformer 存在问题？
    16. Transformer 怎么 Coding?
  - [【关于 Transformer-XL】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/T3_Transformer_XL/)
    - 动机
      - RNN：主要面临梯度消失或爆炸（gradient vanishing and explosion），解决方法集中在优化方法、初始化策略、辅助记忆单元的研究上。
      - vanilla Transformer：最长建模长度是固定的，无法捕捉更长依赖关系；等长输入序列的获取通常没有遵循句子或语义边界（出于高效考虑，往往就是将文本按长度一段段截取，而没有采用padding机制），可能造成上下文碎片化（context fragmentation）。
    - 方法
      - 引入循环机制（Reccurrence，让上一segment的隐含状态可以传递到下一个segment）：将循环（recurrence）概念引入了深度自注意力网络。不再从头计算每个新segment的隐藏状态，而是复用从之前segments中获得的隐藏状态。被复用的隐藏状态视为当前segment的memory，而当前的segment为segments之间建立了循环连接（recurrent connection）。因此，超长依赖性建模成为了可能，因为信息可以通过循环连接来传播。
      - 提出一种新的相对位置编码方法，避免绝对位置编码在循环机制下的时序错乱：从之前的segment传递信息也可以解决上下文碎片化的问题。更重要的是，本文展示了使用相对位置而不是用绝对位置进行编码的必要性，这样做可以在不造成时间混乱（temporal confusion）的情况下，实现状态的复用。因此，作为额外的技术贡献，文本引入了简单但有效的相对位置编码公式，它可以泛化至比在训练过程中观察到的长度更长的注意力长度。
  - [【关于 SHA_RNN】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/SHA_RNN_study/)
    - 论文名称：Single Headed Attention RNN: Stop Thinking With Your Head 单头注意力 RNN: 停止用你的头脑思考
  - [【关于 Universal Transformers】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/T4_Universal_Transformers/)
  - [【关于Style_Transformer】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/Style_Transformer/LCNQA/)
  - [【关于 Linformer 】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/ACL2020_Linformer)
    - 论文标题：《Linformer: Self-Attention with Linear Complexity》
    - 来源：ACL 2020
    - 链接：https://arxiv.org/abs/2006.04768
    - 参考：https://zhuanlan.zhihu.com/p/149890569
  - [【关于 Performer 】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_study/Performer) **【推荐阅读】**
    - 阅读理由：Transformer 作者 Krzysztof Choromanski 针对 Transformer 问题的重新思考与改进
    - 动机：Transformer 有着巨大的内存和算力需求，因为它构造了一个注意力矩阵，需求与输入呈平方关系;
    - 思路：使用一个高效的（线性）广义注意力框架（generalized attention framework），允许基于不同相似性度量（核）的一类广泛的注意力机制。
    - 优点：该方法在保持线性空间和时间复杂度的同时准确率也很有保证，也可以应用到独立的 softmax 运算。此外，该方法还可以和可逆层等其他技术进行互操作。
  - [【关于 Efficient Transformers: A Survey】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/transformer_survey/Performer)
    - 一、摘要
    - 二、Transformer 介绍
    - 三、Efficient Transformers
      - 3.1 Fixed patterns（FP）
        - 3.1.1 Fixed patterns（FP） 介绍
        - 3.1.2 Fixed patterns（FP） 类别
      - 3.2 Combination of Patterns (CP)
        - 3.2.1 Combination of Patterns (CP) 介绍
        - 3.2.2 Combination of Patterns (CP)  类别
        - 3.2.3 Fixed patterns（FP） vs 多Combination of Patterns (CP)
      - 3.3 Learnable Patterns (LP)
        - 3.3.1 Learnable Patterns (LP) 介绍
        - 3.3.2 Learnable Patterns (LP)  类别
        - 3.3.3 Learnable Patterns (LP)  优点
      - 3.4 Memory
        - 3.4.1 Memory 介绍
        - 3.4.2 Memory 类别
      - 3.5 Low-Rank 方法
        - 3.5.1 Low-Rank 方法 介绍
        - 3.5.2 Low-Rank 方法 类别
      - 3.6 Kernels 方法
        - 3.6.1  Kernels 方法 介绍
        - 3.6.2  Kernels 方法 代表
      - 3.7  Recurrence 方法
        - 3.7.1  Recurrence 方法 介绍
        - 3.7.2  Kernels 方法 代表
    - 四、Transformer 变体 介绍
      - 4.1 引言
      - 4.2 Memory Compressed Transformer 
      - 4.3 Image Transformer 
      - 4.4 Set Transformer 
      - 4.5 Sparse Transformer
      - 4.6 Axial Transformer
      - 4.7 Longformer
      - 4.8  Extended Transformer Construction (ETC)（2020）
      - 4.9  BigBird（2020）
      - 4.10  Routing Transformer
      - 4.11  Reformer（2020）
      - 4.12  Sinkhorn Transformers
      - 4.13  Linformer
      - 4.14   Linear Transformer
      - 4.15  Performer（2020）
      - 4.16  Synthesizer models（2020）
      - 4.17  Transformer-XL（2020）
      - 4.18  Compressive Transformers
    - 五、总结

##### 【关于 Dropout】 那些你不知道的事

- [【关于 R-Drop】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/Dropout/R-Drop/)  
  - 论文：R-Drop: Regularized Dropout for Neural Networks
  - 论文下载地址：https://arxiv.org/abs/2106.14448
  - 论文代码：https://github.com/dropreg/R-Drop
  - 论文动机：
    - 由于深度神经网络非常容易过拟合，因此 Dropout 方法采用了随机丢弃每层的部分神经元，以此来避免在训练过程中的过拟合问题。**正是因为每次随机丢弃部分神经元，导致每次丢弃后产生的子模型都不一样，所以 Dropout 的操作一定程度上使得训练后的模型是一种多个子模型的组合约束。**基于 Dropout 的这种特殊方式对网络带来的随机性，研究员们提出了 R-Drop 来进一步对（子模型）网络的输出预测进行了正则约束。
  - 论文方法：与传统作用于神经元（Dropout）或者模型参数（DropConnect）上的约束方法不同，R-Drop **作用于模型的输出层**，弥补了 Dropout 在训练和测试时的不一致性。简单来说就是在每个 mini-batch 中，**每个数据样本过两次带有 Dropout 的同一个模型，R-Drop 再使用 KL-divergence 约束两次的输出一致**。
  - 作用：**R-Drop 约束了由于 Dropout 带来的两个随机子模型的输出一致性**。

##### 【关于 预训练模型】 那些的你不知道的事

- [【关于Bert】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/)：Bert论文研读
  - [【关于Bert】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/T1_bert/)
    - 阅读理由：NLP 的 创世之作
    - 动机：word2vec 的多义词问题 && GPT 单向 Transformer && Elmo 双向LSTM 
    - 介绍：Transformer的双向编码器
    - 思路：
      - 预训练：Task 1：Masked LM && Task 2：Next Sentence Prediction
      - 微调：直接利用 特定任务数据 微调
    - 优点：NLP 所有任务上都刷了一遍 SOTA
    - 缺点：
      - [MASK]预训练和微调之间的不匹配
      - Max Len 为 512
    - [【关于SpanBert】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/T1_bert/)
      - 论文：SpanBERT: Improving Pre-training by Representing and Predicting Spans
      - 论文地址：https://arxiv.org/abs/1907.10529
      - github：https://github.com/facebookresearch/SpanBERT
      - 动机：旨在更好地表示和预测文本的 span;
      - 论文方法->扩展了BERT：
        - （1）屏蔽连续的随机 span，而不是随机标记；
        - （2）训练 span 边界表示来预测屏蔽 span 的整个内容，而不依赖其中的单个标记表示。
  - [【关于 XLNet 】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/T2_XLNet/)
    - 阅读理由：Bert 问题上的改进
    - 动机：
      - Bert 预训练和微调之间的不匹配
      - Bert 的 Max Len 为 512
    - 介绍：广义自回归预训练方法
    - 思路：
      - 预训练：
        - Permutation Language Modeling【解决Bert 预训练和微调之间的不匹配】
        - Two-Stream Self-Attention for Target-Aware Representations【解决PLM出现的目标预测歧义】 
        - XLNet将最先进的自回归模型Transformer-XL的思想整合到预训练中【解决 Bert 的 Max Len 为 512】
      - 微调：直接利用 特定任务数据 微调
    - 优点：
    - 缺点：
  - [【关于 RoBERTa】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/T4_RoBERTa/) 
    - 阅读理由：Bert 问题上的改进
    - 动机：
      - 确定方法的哪些方面贡献最大可能是具有挑战性的
      - 训练在计算上是昂贵的的，限制了可能完成的调整量
    - 介绍：A Robustly Optimized BERT Pretraining Approach 
    - 思路：
      - 预训练：
        - 去掉下一句预测(NSP)任务
        - 动态掩码
        - 文本编码
      - 微调：直接利用 特定任务数据 微调
    - 优点：
    - 缺点：
  - [【关于 ELECTRA 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/ELECTRA/)
    - 阅读理由：Bert 问题上的改进 【不推荐阅读，存在注水！】
    - 动机：
      - 只有15%的输入上是会有loss
    - 介绍：判别器 & 生成器 【但是最后发现非 判别器 & 生成器】
    - 思路：
      - 预训练：
        - 利用一个基于MLM的Generator来替换example中的某些个token，然后丢给Discriminator来判别
      - 微调：直接利用 特定任务数据 微调
    - 优点：
    - 缺点： 
  - [【关于 Perturbed Masking: Parameter-free Probing for Analyzing and Interpreting BERT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/ACL2020_UnsupervisedBert/)
    - 论文链接：https://arxiv.org/pdf/2004.14786.pdf
    - 代码链接：https://github.com/bojone/perturbed_masking
    - 动机
      - 通过引入少量的附加参数，probe learns 在监督方式中使用特征表示（例如，上下文嵌入）来 解决特定的语言任务（例如，依赖解析）。这样的probe  tasks 的有效性被视为预训练模型编码语言知识的证据。但是，这种评估语言模型的方法会因 probe 本身所学知识量的不确定性而受到破坏
    - Perturbed Masking 
      - 介绍：parameter-free probing technique
      - 目标：analyze and interpret pre-trained models，测量一个单词xj对预测另一个单词xi的影响，然后从该单词间信息中得出全局语言属性（例如，依赖树）。
    - 整体思想很直接，句法结构，其实本质上描述的是词和词之间的某种关系，如果我们能从BERT当中拿到词和词之间相互“作用”的信息，就能利用一些算法解析出句法结构。
  - [【关于 GRAPH-BERT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/bert_study/T2020_GRAPH_BERT))
    - 论文名称：GRAPH-BERT: Only Attention is Needed for Learning Graph Representations
    - 论文地址：https://arxiv.org/abs/2001.05140
    - 论文代码：https://github.com/jwzhanggy/Graph-Bert
    - 动机
      - 传统的GNN技术问题：
        - 模型做深会存在suspended animation和over smoothing的问题。
        - 由于 graph 中每个结点相互连接的性质，一般都是丢进去一个完整的graph给他训练而很难用batch去并行化。
    - 方法：提出一种新的图神经网络模型GRAPH-BERT (Graph based BERT)，该模型只依赖于注意力机制，不涉及任何的图卷积和聚合操作。Graph-Bert 将原始图采样为多个子图，并且只利用attention机制在子图上进行表征学习，而不考虑子图中的边信息。因此Graph-Bert可以解决上面提到的传统GNN具有的性能问题和效率问题。
  - [【关于自训练 + 预训练 = 更好的自然语言理解模型 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/bert_study/SelfTrainingImprovesPreTraining))
    - 论文标题：Self-training Improves Pre-training for Natural Language Understanding
    - 论文地址：https://arxiv.org/abs/2010.02194
    - 动机 
      - 问题一: do  pre-training and self-training capture the same information,  or  are  they  complementary?
      - 问题二: how can we obtain large amounts of unannotated data from specific domains?
    - 方法
      - 问题二解决方法：提出 SentAugment 方法 从 web 上获取有用数据；
      - 问题一解决方法：使用标记的任务数据训练一个 teacher 模型，然后用它对检索到的未标注句子进行标注，并基于这个合成数据集训练最终的模型。

- [【关于 Bert 模型压缩】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/Bert_zip)
  - [【关于 Bert 模型压缩】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/Bert_zip)
    - 阅读理由：Bert 在工程上问题上的改进 
    - 动机：
      - 内存占用；
      - 功耗过高；
      - 带来很高的延迟；
      - 限制了 Bert 系列模型在移动和物联网等嵌入式设备上的部署；
    - 介绍：BERT 瘦身来提升速度
    - 模型压缩思路：
      - 低秩因式分解：在输入层和输出层使用嵌入大小远小于原生Bert的嵌入大小，再使用简单的映射矩阵使得输入层的输出或者最后一层隐藏层的输出可以通过映射矩阵输入到第一层的隐藏层或者输出层；
      - 跨层参数共享：隐藏层中的每一层都使用相同的参数，用多种方式共享参数，例如只共享每层的前馈网络参数或者只共享每层的注意力子层参数。默认情况是共享每层的所有参数；
      - 剪枝：剪掉多余的连接、多余的注意力头、甚至LayerDrop[1]直接砍掉一半Transformer层
      - 量化：把FP32改成FP16或者INT8；
      - 蒸馏：用一个学生模型来学习大模型的知识，不仅要学logits，还要学attention score；
    - 优点：BERT 瘦身来提升速度
    - 缺点： 
      - 精度的下降
      - 低秩因式分解 and 跨层参数共享 计算量并没有下降；
      - 剪枝会直接降低模型的拟合能力；
      - 量化虽然有提升但也有瓶颈；
      - 蒸馏的不确定性最大，很难预知你的BERT教出来怎样的学生；
  - [【关于 Distilling Task-Specific Knowledge from BERT into Simple Neural Networks】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/BERTintoSimpleNeuralNetworks/)
    - 动机：
      - 随着 BERT 的横空出世，意味着 上一代用于语言理解的较浅的神经网络（RNN、CNN等） 的 过时？
      - BERT模型是真的大，计算起来太慢了？
      - 是否可以将BERT（一种最先进的语言表示模型）中的知识提取到一个单层BiLSTM 或 TextCNN 中？
    - 思路：
        1. 确定 Teacher 模型（Bert） 和 Student 模型（TextCNN、TextRNN）;
        2. 蒸馏的两个过程：
           1. 第一，在目标函数附加logits回归部分；
           2. 第二，构建迁移数据集，从而增加了训练集，可以更有效地进行知识迁移。
  - [【关于 AlBert 】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/T5_ALBERT/)
    - 模型压缩方法：低秩因式分解 + 跨层参数共享
    - 模型压缩方法介绍：
      - 低秩因式分解：
        - 动机：Bert的参数量大部分集中于模型的隐藏层架构上，在嵌入层中只有30,000词块，其所占据的参数量只占据整个模型参数量的小部分；
        - 方法：将输入层和输出层的权重矩阵分解为两个更小的参数矩阵；
        - 思路：在输入层和输出层使用嵌入大小远小于原生Bert的嵌入大小，再使用简单的映射矩阵使得输入层的输出或者最后一层隐藏层的输出可以通过映射矩阵输入到第一层的隐藏层或者输出层；
        - 优点：在不显著增加词嵌入大小的情况下能够更容易增加隐藏层大小；
      - 参数共享【跨层参数共享】：
        - 动机：隐藏层 参数 大小 一致；
        - 方法：隐藏层中的每一层都使用相同的参数，用多种方式共享参数，例如只共享每层的前馈网络参数或者只共享每层的注意力子层参数。默认情况是共享每层的所有参数；
        - 优点：防止参数随着网络深度的增加而增大；
    - 其他改进策略：
      - **句子顺序预测损失(SOP)**代替**Bert中的下一句预测损失(NSP)**：
        - 动机：通过实验证明，Bert中的下一句预测损失(NSP) 作用不大；
        - 介绍：用预测两个句子是否连续出现在原文中替换为两个连续的句子是正序或是逆序，用于进一步提高下游任务的表现
    - 优点：参数量上有所降低；
    - 缺点：其加速指标仅展示了训练过程，由于ALBERT的隐藏层架构**采用跨层参数共享策略并未减少训练过程的计算量**，加速效果更多来源于低维的嵌入层；
  - [【关于 FastBERT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/FastBERT/)
    - 模型压缩方法：知识蒸馏
    - 模型压缩方法介绍：
      - 样本自适应机制（Sample-wise adaptive mechanism）
        - 思路：
          - 在每层Transformer后都去预测样本标签，如果某样本预测结果的置信度很高，就不用继续计算了，就是自适应调整每个样本的计算量，容易的样本通过一两层就可以预测出来，较难的样本则需要走完全程。
        - 操作：
          - 给每层后面接一个分类器，毕竟分类器比Transformer需要的成本小多了
      - 自蒸馏（Self-distillation）
        - 思路：
          - 在预训练和精调阶段都只更新主干参数；
          - 精调完后freeze主干参数，用分支分类器（图中的student）蒸馏主干分类器（图中的teacher）的概率分布
        - 优点：
          - 非蒸馏的结果没有蒸馏要好
          - 不再依赖于标注数据。蒸馏的效果可以通过源源不断的无标签数据来提升
  - [【关于 distilbert】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/distilbert/)
  - [【关于 TinyBert】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/TinyBERT/)
    - 模型压缩方法：知识蒸馏
    - tinybert的创新点：学习了teacher Bert中更多的层数的特征表示；
    - 模型压缩方法介绍：
      - 基于transformer的知识蒸馏模型压缩
        - 学习了teacher Bert中更多的层数的特征表示；
        - 特征表示：
          - 词向量层的输出；
          - Transformer layer的输出以及注意力矩阵；
          - 预测层输出(仅在微调阶段使用)；
      - bert知识蒸馏的过程
        - 左图：整体概括了知识蒸馏的过程
          - 左边：Teacher BERT；
          - 右边：Student TinyBERT
          - 目标：将Teacher BERT学习到的知识迁移到TinyBERT中
        - 右图：描述了知识迁移的细节；
          - 在训练过程中选用Teacher BERT中每一层transformer layer的attention矩阵和输出作为监督信息
- [【关于 Perturbed Masking】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/bert_study/ACL2020_UnsupervisedBert)
  - 论文：Perturbed Masking: Parameter-free Probing for Analyzing and Interpreting BERT
  - 论文链接：https://arxiv.org/pdf/2004.14786.pdf
  - 代码链接：https://github.com/bojone/perturbed_masking
  - 动机： 通过引入少量的附加参数，probe learns 在监督方式中使用特征表示（例如，上下文嵌入）来 解决特定的语言任务（例如，依赖解析）。这样的probe  tasks 的有效性被视为预训练模型编码语言知识的证据。但是，这种评估语言模型的方法会因 probe 本身所学知识量的不确定性而受到破坏。
  - 方法介绍：
    - Perturbed Masking 
      - 介绍：parameter-free probing technique
      - 目标：analyze and interpret pre-trained models，测量一个单词xj对预测另一个单词xi的影响，然后从该单词间信息中得出全局语言属性（例如，依赖树）。
  - 思想：整体思想很直接，句法结构，其实本质上描述的是词和词之间的某种关系，如果我们能从BERT当中拿到词和词之间相互“作用”的信息，就能利用一些算法解析出句法结构。 

- [【关于中文预训练模型】那些你不知道的事]((https://github.com/km1994/nlp_paper_study/tree/master/bert_study/Chinese/)
  - [【关于ChineseBERT】那些你不知道的事]((https://github.com/km1994/nlp_paper_study/tree/master/bert_study/Chinese/ChineseBERT/)
  - 论文名称：ChineseBERT: Chinese Pretraining Enhanced by Glyph and Pinyin Information
  - 会议： ACL2021
  - 论文地址：https://arxiv.org/abs/2106.16038
  - 论文源码地址：https://github.com/ShannonAI/ChineseBert
  - 模型下载：https://huggingface.co/hfl/chinese-bert-wwm-ext/tree/main
  - 动机：最近的中文预训练模型忽略了中文特有的两个重要方面：字形和拼音，它们为语言理解携带重要的句法和语义信息。
  - 论文工作：提出了 ChineseBERT，它将汉字的 {\it glyph} 和 {\it pinyin} 信息合并到语言模型预训练中。
    - embedding 层：将 字符嵌入（char embedding）、字形嵌入（glyph embedding）和拼音嵌入（pinyin embedding） 做拼接；
    - Fusion Layer 层：将 拼接后的 embedding 向量 做 Fusion 得到 一个 d 维的 Fusion embedding;
    - 位置拼接：将 Fusion embedding 和 位置嵌入（position embedding）、片段嵌入（segment embedding）相加；
    - Transformer-Encoder层;
  - 改进点：
    - 在底层的融合层（Fusion Layer）融合了除字嵌入（Char Embedding）之外的字形嵌入（Glyph Embedding）和拼音嵌入（Pinyin Embedding），得到融合嵌入（Fusion Embedding），再与位置嵌入相加，就形成模型的输入；
    - 抛弃预训练任务中的NSP任务。 由于预训练时没有使用NSP任务，因此模型结构图省略了片段嵌入（segment embedding）。实际上下游任务输入为多个段落时（例如：文本匹配、阅读理解等任务），是采用了segment embedding；
  - 实验结果：在大规模未标记的中文语料库上进行预训练，提出的 ChineseBERT 模型在训练步骤较少的情况下显着提高了基线模型的性能。 porpsoed 模型在广泛的中文 NLP 任务上实现了新的 SOTA 性能，包括机器阅读理解、自然语言推理、文本分类、句子对匹配和命名实体识别中的竞争性能。

##### [【关于 信息抽取】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/)

###### [【关于 实体关系联合抽取】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/ERE_study/)

- [【关于 A Frustratingly Easy Approach for Joint Entity and Relation Extraction】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/ERE_study/AFrustratinglyEasyApproachForJEandRE/) 【强烈推荐】
  - 论文：A Frustratingly Easy Approach for Joint Entity and Relation Extraction
  - 阅读理由：反直觉！陈丹琦用pipeline方式刷新关系抽取SOTA 
  - 方法：建立两个 encoders，并独立训练:
    - encoder 1：entity model
      - 方法：建立在 span-level representations 上
    - encoder 2：relation model：只依赖于实体模型作为输入特征
      - 方法：builds on contextual representations specific to a given pair of span
  - 优点：
    - 很简单，但我们发现这种流水线方法非常简单有效；
    - 使用同样的预先训练的编码器，我们的模型在三个标准基准（ACE04，ACE05，SciERC）上优于所有以前的联合模型；
  - 问题讨论：
    - Q1、关系抽取最care什么？
      - 解答：引入实体类别信息会让你的关系模型有提升
    - Q2、共享编码 VS 独立编码 哪家强？
      -  解答：由于两个任务各自是不同的输入形式，并且需要不同的特征去进行实体和关系预测，也就是说：使用单独的编码器确实可以学习更好的特定任务特征。
    - Q3：误差传播不可避免？还是不存在？
      - 解答：并不认为误差传播问题不存在或无法解决，而需要探索更好的解决方案来解决此问题
    - Q4：Effect of Cross-sentence Context
      - 解答：使用跨句上下文可以明显改善实体和关系
- [【关于 实体关系联合抽取】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/ERE_study/实体关系联合抽取总结.md)
- [Incremental Joint Extraction of Entity Mentions and Relations](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/ERE_study/T2014_joint_extraction/)
- [【关于 Joint NER】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/ERE_study/JointER/)
  - 论文名称：Joint Extraction of Entities and Relations Based on a Novel Decomposition Strategy
- [【关于 GraphRel】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/ERE_study/ACL2019_GraphRel/)
  - 论文名称：论文名称：GraphRel: Modeling Text as Relational Graphs for Joint Entity and Relation Extraction
  - 动机
    - 想要自动提取特征的联合模型
      - 通过堆叠Bi-LSTM语句编码器和GCN (Kipf和Welling, 2017)依赖树编码器来自动学习特征
      - 用以考虑线性和依赖结构
        - 类似于Miwa和Bansal(2016)（一样是堆叠的）
          - 方法
            - 每个句子使用Bi-LSTM进行自动特征学习
            - 提取的隐藏特征由连续实体标记器和最短依赖路径关系分类器共享
          - 问题
            - 然而，在为联合实体识别和关系提取引入共享参数时：
              - 它们仍然必须将标记者预测的实体提及通过管道连接起来
              - 形成关系分类器的提及对
      - 考虑重叠关系
      - 如何考虑关系之间的相互作用
        - 2nd-phase relation-weighted GCN
        - 重叠关系(常见）
          - 情况
            - 两个三元组的实体对重合
            - 两个三元组都有某个实体mention
          - 推断
            - 困难（对联合模型尤其困难，因为连实体都还不知道）
    - 方法：
      - 学习特征
        - 通过堆叠Bi-LSTM语句编码器和GCN (Kipf和Welling, 2017)依赖树编码器来自动学习特征
      - 第一阶段的预测
        - GraphRel标记实体提及词，预测连接提及词的关系三元组
        - 用关系权重的边建立一个新的全连接图（中间图）
        - 指导：关系损失和实体损失
      - 第二阶段的GCN
        - 通过对这个中间图的操作
        - 考虑实体之间的交互作用和可能重叠的关系
        - 对每条边进行最终分类
        - 在第二阶段，基于第一阶段预测的关系，我们为每个关系构建完整的关系图，并在每个图上应用GCN来整合每个关系的信息，进一步考虑实体与关系之间的相互作用。
- [【关于 关系抽取 之 HBT】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/ERE_study/T20ACL_HBT_su/)
  - 论文名称：A Novel Hierarchical Binary Tagging Framework for Relational Triple Extraction
  - 论文会议：ACL 2020
  - keras4bert 版本：https://github.com/bojone/lic2020_baselines 【苏神 Lic2020 baseline】
  - pytorch 版本：https://github.com/powerycy/Lic2020- 【逸神 pytorch 复现版本】
  - 动机：
    - pipeline approach
      - 思路
        - 实体抽取：利用一个命名实体识别模型 识别句子中的所有实体；
        - 关系分类：利用 一个关系分类模型 对每个实体对执行关系分类。 【这一步其实可以理解为文本分类任务，但是和文本分类任务的区别在于，关系分类不仅需要学习句子信息，还要知道 实体对在 句子中 位置信息】 
      - 问题
        - 误差传递问题：由于 该方法将 实体-关系联合抽取任务 分成 实体抽取+关系分类 两个任务处理，所以 实体抽取任务的错误无法在后期阶段进行纠正，因此这种方法容易遭受错误传播问题；
    - feature-based models and neural network-based models 
      - 思路
        - 通过用学习表示替换人工构建的特征，基于神经网络的模型在三重提取任务中取得了相当大的成功。
      - 问题
        - 大多数现有方法无法正确处理句子包含多个相互重叠的关系三元组的情况。
    - 基于Seq2Seq模型  and GCN
      - 思路：
        - 提出了具有复制机制以提取三元组的序列到序列（Seq2Seq）模型。 他们基于Seq2Seq模型，进一步研究了提取顺序的影响，并通过强化学习获得了很大的改进。 
      - 问题：
        - 过多 negative examples：在所有提取的实体对中，很多都不形成有效关系，从而产生了太多的negative examples；
        - EPO(Entity Pair Overlap) 问题：当同一实体参与多个关系时，分类器可能会感到困惑。 没有足够的训练样例的情况下，分类器就很难准确指出实体参与的关系；
  - 方式：实现了一个不受重叠三元组问题困扰的HBT标注框架(Hierarchical Binary Tagging Framework)来解决RTE任务；论文并不是学习关系分类器f（s，o）→r，而是学习关系特定的标记器fr（s）→o；每个标记器都可以识别特定关系下给定 subject 的可能 object(s)。 或不返回任何 object，表示给定的主题和关系没有 triple。
  - 核心思想：把关系(Relation)建模为将头实体(Subject)映射到尾实体(Object)的函数，而不是将其视为实体对上的标签。
  - 思路：
    - 首先，我们确定句子中所有可能的 subjects； 
    - 然后针对每个subjects，我们应用特定于关系的标记器来同时识别所有可能的 relations 和相应的 objects。
  - 结构：
    - BERT Encoder层：使用 Bert 做 Encoder，其实就是 用 Bert 做 Embedding 层使用。
    - Hierarchical Decoder层
      - Subject tagger 层：用于 提取 Subject;
      - Relation-Specific Object Taggers 层：由一系列relation-specific object taggers（之所以这里是多个taggers是因为有多个可能的relation）；

###### [【关于 命名实体识别】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/)

- [【关于 Continual Learning for NER】那些你不知道的事](#关于-continual-learning-for-ner那些你不知道的事)
  - 会议：AAAI2021
  - 论文：Continual Learning for Named Entity Recognition
  - 论文下载地址：https://assets.amazon.science/65/61/ecffa8df45ad818c3f69fb1cf72b/continual-learning-for-named-entity-recognition.pdf
  - 动机：业务扩展，需要新增 实体类型（eg:像 Sirior Alexa 这样的语音助手不断地为其功能引入新的意图，因此**新的实体类型经常被添加到他们的插槽填充模型**中）
  - 方法：研究 将 知识蒸馏（KD） 应用于 NER 的 CL 问题，通过 将 “teacher”模型的预测合并到“student”模型的目标函数中，该模型正在接受训练以执行类似但略有修改的任务。 通过学习输出概率分布，而不仅仅是标签，使得学生表现得与教师相似。
  - 论文贡献：
    - (i) 我们展示了如何使 CL 技术适应 NLU 域，以逐步学习 NER 的新实体类型； 
    - (ii) 我们在两个 EnglishNER 数据集上的结果表明，我们的 CL 方法使模型能够不断学习新的实体类型，而不会失去识别先前获得的类型的能力； 
    - (iii) 我们表明我们的半监督策​​略实现了与全监督设置相当的结果。

- [【关于 NER数据存在漏标问题】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/UnlabeledEntityProblem/)
  - 一、摘要
  - 二、为什么 数据会存在漏标？
  - 三、什么是 带噪学习
  - 四、NER 数据漏标问题所带来后果？
  - 五、NER 性能下降 **原因**是什么？
  - 六、论文所提出的方法是什么？
  - 七、数据漏标，会导致NER指标下降有多严重？
  - 八、对「未标注实体问题」的解决方案有哪些？
  - 九、如何降噪：改变标注框架+负采样？
    - 9.1 第一步：改变标注框架
    - 9.2 第二步：负采样
  - 十、负样本采样，效果如何？
- [【关于 LEX-BERT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ICLR2021_LEX_BERT/)【强烈推荐】
  - 推荐理由：在 query 中 引入 标签信息的方法，秒杀 Flat NER，登上 2021 年 Chinese NER SOTA。
  - 论文名称：《Lex-BERT: Enhancing BERT based NER with lexicons》
  - 动机：尽管它在NER任务中的表现令人印象深刻，但最近已经证明，添加词汇信息可以显著提高下游性能。然而，没有任何工作在不引入额外结构的情况下将单词信息纳入BERT。在我们的工作中，我们提出了词法BERT（lex-bert），这是一种在基于BERT的NER模型中更方便的词汇借用方法
  - 方法：
    - LEX-BERT V1：Lex BERT的第一个版本通过在单词的左右两侧插入特殊标记来识别句子中单词的 span。特殊标记不仅可以标记单词的起始位置和结束位置，还可以为句子提供实体类型信息
    - LEX-BERT V2：对于在句子中加宽的单词，我们没有在句子中单词的周围插入起始和结束标记，而是在句子的末尾附加一个标记[x]。请注意，我们将标记的位置嵌入与单词的起始标记绑定
- [【关于 嵌套命名实体识别（Nested NER）】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/NestedNER/)
  - [【关于 Biaffine Ner 】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ACL2020_NERasDependencyParsing/)
    - 动机：NER 研究 关注于 扁平化NER，而忽略了 实体嵌套问题；
    - 方法： 在本文中，我们使用基于图的依存关系解析中的思想，以通过 biaffine model 为模型提供全局的输入视图。 biaffine model 对句子中的开始标记和结束标记对进行评分，我们使用该标记来探索所有跨度，以便该模型能够准确地预测命名实体。
    - 工作介绍：在这项工作中，我们将NER重新确定为开始和结束索引的任务，并为这些对定义的范围分配类别。我们的系统在多层BiLSTM之上使用biaffine模型，将分数分配给句子中所有可能的跨度。此后，我们不用构建依赖关系树，而是根据候选树的分数对它们进行排序，然后返回符合 Flat 或  Nested NER约束的排名最高的树 span；
    - 实验结果：我们根据三个嵌套的NER基准（ACE 2004，ACE 2005，GENIA）和五个扁平的NER语料库（CONLL 2002（荷兰语，西班牙语），CONLL 2003（英语，德语）和ONTONOTES）对系统进行了评估。结果表明，我们的系统在所有三个嵌套的NER语料库和所有五个平坦的NER语料库上均取得了SoTA结果，与以前的SoTA相比，实际收益高达2.2％的绝对百分比。
  - [【关于 Biaffine 代码解析】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ACL2020_NERasDependencyParsing/code_pytorch.md)
    - 摘要
    - 一、数据处理模块
      - 1.1 原始数据格式
      - 1.2 数据预处理模块 data_pre()
        - 1.2.1 数据预处理 主 函数
        - 1.2.2  训练数据加载 load_data(file_path)
        - 1.2.3 数据编码 encoder(sentence, argument)
      - 1.3 数据转化为 MyDataset 对象
      - 1.4 构建 数据 迭代器
      - 1.5 最后数据构建格式
    - 二、模型构建 模块
      - 2.1 主题框架介绍
      - 2.2 embedding layer
      - 2.2 BiLSTM
      - 2.3 FFNN
      - 2.4 biaffine model
      - 2.5 冲突解决
      - 2.6 损失函数
    - 三、学习率衰减 模块
    - 四、loss 损失函数定义
      - 4.1 span_loss 损失函数定义
      - 4.2 focal_loss 损失函数定义
    - 四、模型训练
- [【关于 NER trick】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/NER_study/NERtrick.md)
- [【关于TENER】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ACL2019/ACL2019_TENER/)
  - 论文名称：TENER: Adapting Transformer Encoder for Name Entity Recognition
  - 动机：
    - 1. Transformer 能够解决长距离依赖问题；
    - 2. Transformer 能够并行化；
    - 3. 然而，Transformer 在 NER 任务上面效果不好。
  - 方法：
    -  第一是经验发现。 引入：相对位置编码
    -  第二是经验发现。 香草变压器的注意力分布是缩放且平滑的。 但是对于NER，因为并非所有单词都需要参加，所以很少注意是合适的。 给定一个当前单词，只需几个上下文单词就足以判断其标签。 平稳的注意力可能包括一些嘈杂的信息。 因此，我们放弃了点生产注意力的比例因子，而使用了无比例且敏锐的注意力。
- [【关于DynamicArchitecture】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/DynamicArchitecture/)
  - 介绍：Dynamic Architecture范式通常需要设计相应结构以融入词汇信息。
  - 论文：
    - [【关于 LatticeLSTM 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/DynamicArchitecture/1_ACL2018_LatticeLSTM/)
      - 想法：在 char-based 的 LSTM 中引入词汇信息
      - 做法：
        - 根据大量语料生成词典；
        - 若当前字符与前面的字符无法组成词典中词汇，则按 LSTM 的方法更新记忆状态；
        - 若当前字符与前面的字符组成词典中词汇，从最新词汇中提取信息，联合更新记忆状态；
      - 存在问题：
        - 计算性能低下，导致其**不能充分利用GPU进行并行化**。究其原因主要是每个字符之间的增加word cell（看作节点）数目不一致；
        - 信息损失：
          - 1）每个字符只能获取以它为结尾的词汇信息，对于其之前的词汇信息也没有持续记忆。如对于「大」，并无法获得‘inside’的「长江大桥」信息。
          - 2）由于RNN特性，采取BiLSTM时其前向和后向的词汇信息不能共享，导致 Lattice LSTM **无法有效处理词汇信息冲突问题**
        - 可迁移性差：只适配于LSTM，不具备向其他网络迁移的特性。
    - [【关于 LR-CNN 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/DynamicArchitecture/2_IJCAI2019_LR_CNN/)
      - 动机
        - 词信息引入问题；
         - lattice LSTM 问题：
           - 基于 RNN 结构方法不能充分利用 GPU 并行计算资源；
             - 针对句子中字符计算；
             - 针对匹配词典中潜在词
           - 很难处理被合并到词典中的潜在单词之间的冲突：
             - 一个字符可能对应词典中多个潜在词，误导模型
       - 方法：
        - Lexicon-Based CNNs：采取CNN对字符特征进行编码，感受野大小为2提取bi-gram特征，堆叠多层获得multi-gram信息；同时采取注意力机制融入词汇信息（word embed）；
        - Refining Networks with Lexicon Rethinking：由于上述提到的词汇信息冲突问题，LR-CNN采取rethinking机制增加feedback layer来调整词汇信息的权值：具体地，将高层特征作为输入通过注意力模块调节每一层词汇特征分布，利用这种方式来利用高级语义来完善嵌入单词的权重并解决潜在单词之间的冲突。
    - [【关于 CGN 】那些你不知道的事 ](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/DynamicArchitecture/3_EMNLP2019_CGN/)
      - 动机
        - 中文命名实体识别中，词边界 问题；
        - 如何 引入 词边界信息：
          - pipeline：CWS -> NER 
            - 问题：误差传递
          - CWS 和 NER 联合学习
            - 问题：标注 CWS 数据
          - 利用 词典 自动构建
            - 优点：比 CWS 标注数据 更容易获得
            - 问题：
              - 第一个挑战是整合自我匹配的词汇词；
                - 举例：“北京机场” (Beijing Airport) and “机场” (Airport) are the self-matched words of the character “机” (airplane)
              - 第二个挑战是直接整合最接近的上下文词汇词；
                - 举例：by directly using the semantic knowledge of the nearest contextual words “离开” (leave), an “I-PER” tag can be predicted instead of an “I-ORG” tag, since “希尔顿” (Hilton Hotels) cannot be taken as the subject of the verb “离开” 
        - 论文思路：
          - character-based Collaborative Graph：
            - encoding layer：
              - 句子信息：
                - s1：将 char 表示为 embedding;
                - s2：利用 biLSTM 捕获 上下文信息
              - lexical words 信息：
                - s1：将 lexical word 表示为 embedding;
              - 合并 contextual representation 和 word embeddings
            - a graph layer：
              - Containing graph (C-graph):
                - 思路：字与字之间无连接，词与其inside的字之间有连接；
                - 目的：帮助 字符 捕获 self-matched lexical words 的边界和语义信息
              - Transition graph (T-graph):
                - 思路：相邻字符相连接，词与其前后字符连接；
                - 目的：帮助 字符 捕获 相邻 上下文 lexical 词 的 语义信息
              - Lattice graph (L-graph):
                - 思路：通相邻字符相连接，词与其开始结束字符相连；
                - 目的：融合 lexical knowledge
              - GAT:
                - 操作：针对三种图，使用Graph Attention Network(GAN)来进行编码。最终每个图的输出
                  - > 其中 $G_k$ 为第k个图的GAN表示，因为是基于字符级的序列标注，所以解码时只关注字符，因此从矩阵中取出前n行作为最终的图编码层的输出。
            - a fusion layer：
              - 目的：融合 三种 graphs 中不同 的 lexical 知识 
            - a decoding layer:
              - 操作：利用 CRF 解码
    - [【关于 LGN 】那些你不知道的事 ](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/DynamicArchitecture/4_EMNLP2019_LGN/)
      - 动机：
        - 在 char-base Chinese NER 中，同一个字符可能属于多个 lexicon word，存在 overlapping ambiguity 问题
          - 举例(如下图)
            - 字符[流] 可以 匹配词汇 [河流] 和 [流经] 两个词汇信息，但是 Lattice LSTM 只能利用 [河流]；
        - Lattice LSTM这种RNN结构仅仅依靠前一步的信息输入，而不是利用全局信息
          - 举例
            - 字符 [度]只能看到前序信息，不能充分利用 [印度河] 信息，从而造成标注冲突问题
        - Ma等人于2014年提出，想解决overlapping across strings的问题，需要引入「整个句子中的上下文」以及「来自高层的信息」；然而，现有的基于RNN的序列模型，不能让字符收到序列方向上 remain characters 的信息；
      - 方法：
        - Graph Construction and Aggregation
        - Graph Construction 
        - Local Aggregation
        - Global Aggregation
        - Recurrent-based Update Module
    - [【关于 FLAT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/DynamicArchitecture/5_ACL2020_FLAT/)
      - 动机
        - 方法一：设计一个动态框架，能够兼容词汇输入；
          - 代表模型： 
            - Lattice LSTM：利用额外的单词单元编码可能的单词，并利用注意力机制融合每个位置的变量节点
            - LR-CNN：采用不同窗口大小的卷积核来编码 潜在词
          - 问题：
            - RNN 和 CNN 难以解决长距离依赖问题，它对于 NER 是有用的，例如： coreference（共指）
            - 无法充分利用 GPU 的并行计算能力
        - 方法二：将 Lattice 转化到图中并使用 GNN 进行编码：
          - 代表模型
            - Lexicon-based GN(LGN)
            - Collaborative GN(CGN)
          - 问题
            - 虽然顺序结构对于NER仍然很重要，并且 Graph 是一般的对应物，但它们之间的差距不可忽略;
            - 需要使用 LSTM 作为底层编码器，带有顺序感性偏置，使模型变得复杂。
      - 方法：将Lattice结构展平，将其从一个有向无环图展平为一个平面的Flat-Lattice Transformer结构，由多个span构成：每个字符的head和tail是相同的，每个词汇的head和tail是skipped的。
- [【关于 ACL 2019 中的NER】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ACL2019/)
  - [named entity recognition using positive-unlabeled learning](https://github.com/km1994/nlp_paper_study/tree/master/NER_study/ACL2019/JointER/)
  - [【关于 GraphRel】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ACL2019/ACL2019_NERusingPositive-unlabeledLearning/)
    - 论文名称：GraphRel: Modeling Text as Relational Graphs for Joint Entity and Relation Extraction
  - [Fine-Grained Entity Typing in Hyperbolic Space（在双曲空间中打字的细粒度实体）](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ACL2019/Fine-GrainedEntityTypinginHyperbolicSpace/)
  - [【关于 TENER】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/ACL2019/ACL2019_TENER/)
    - 论文名称：TENER: Adapting Transformer Encoder for Name Entity Recognition
- [【关于 EMNLP 2019 中的NER】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/EMNLP2019/)
  - [CrossWeigh从不完善的注释中训练命名实体标注器](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/EMNLP2019/CrossWeigh从不完善的注释中训练命名实体标注器/)
  - [利用词汇知识通过协同图网络进行中文命名实体识别](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/EMNLP2019/利用词汇知识通过协同图网络进行中文命名实体识别/)
  - [一点注释对引导低资源命名实体识别器有很多好处](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NER_study/EMNLP2019/一点注释对引导低资源命名实体识别器有很多好处/)


###### [【关于 关系抽取】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/)

- [End-to-End Relation Extraction using LSTMs on Sequences and Tree Structures【2016】](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/T2016_LSTM_Tree/)
- [【关于 ERNIE】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/NRE_paper_study/ERNIE/)
- [【关于 GraphRel】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/GraphRel/)
- [【关于 R_BERT】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/R_BERT)
- [【关于 Task 1：全监督学习】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/T1_FullySupervisedLearning/)
  - [Relation Classification via Convolutional Deep Neural Network](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/T1_FullySupervisedLearning/T1_Relation_Classification_via_CDNN/)
  - [Attention-Based Bidirectional Long Short-Term Memory Networks for Relation Classification](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/T1_FullySupervisedLearning/T2_Attention-Based_BiLSTM_for_RC/)
  - [Relation Classification via Attention Model](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/information_extraction/NRE_paper_study/T1_FullySupervisedLearning/T3_RC_via_attention_model_new/)
- [【关于 Task 2：远程监督学习】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/T2_DistantSupervisedLearning/)
  - [Relation Classification via Convolutional Deep Neural Network](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/T2_DistantSupervisedLearning/T1_Piecewise_Convolutional_Neural_Networks/)
  - [NRE_with_Selective_Attention_over_Instances](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/NRE_paper_study/T2_DistantSupervisedLearning/T2_NRE_with_Selective_Attention_over_Instances/)

###### [【关于 文档级别关系抽取】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/Doc-level_Relation_Extraction/)

- [【关于 Double Graph Based Reasoning for Document-level Relation Extraction】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/Doc-level_Relation_Extraction/DoubleGraphBasedReasoningforDocumentlevelRelationExtraction/)
- [【关于 ATLOP】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/Doc-level_Relation_Extraction/ATLOP/)
  - 论文：Document-Level Relation Extraction with Adaptive Thresholding and Localized Context Pooling
  - 发表会议：AAAI
  - 论文地址：https://arxiv.org/abs/2010.11304
  - github：https://github.com/wzhouad/ATLOP
  - 论文动机：
    - 对于文档级RE，一个文档包含多个实体对，需要同时对它们之间的关系进行分类 【语句级RE只包含一对实体对】
    - 对于文档级RE，一个实体对可以在与不同关系关联的文档中多次出现【对于句子级RE，每个实体对只能出现一个关系】 -> 多标签问题
    - 目前对于文档关系抽取主流的做法是采用基于graph的方法来做，但是很多基于BERT的工作也能够得到很好的结果，并且在基于graph的模型的实验部分，也都证明了BERT以及BERT-like预训练模型的巨大提升，以至于让人怀疑是否有必要引入GNN？作者发现如果只用BERT的话，那么对于不同的entity pair，entity的rep都是一样的，这是一个很大的问题，那是否能够不引入graph的方式来解决这个问题呢？
  - 论文方法：
    - localized context pooling
      - 解决问题：解决了 using the same entity embedding for allentity pairs 问题
      - 方法：使用与当前实体对相关的额外上下文来增强 entity embedding。不是从头开始训练一个new context attention layer ，而是直接将预先训练好的语言模型中的注意头转移到实体级的注意上
    - adaptive thresholding
      - 解决问题：问题 1 的 多实体对问题 和 问题 2 实体对存在多种关系问题
      - 方法：替换为先前学习中用于多标签分类的全局阈值，该阈值为**可学习的依赖实体的阈值**。

###### [【关于 事件抽取】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/event_extraction/)

- [【关于 MLBiNet】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/information_extraction/event_extraction/MLBiNet/)
  - 论文：MLBiNet: A Cross-Sentence Collective Event Detection Network
  - 会议： ACL2021
  - 论文下载地址：https://arxiv.org/pdf/2105.09458.pdf
  - 论文代码：https://github.com/zjunlp/DocED
  - 动机：跨句事件抽取旨在研究如何同时识别篇章内多个事件
  - 论文方法：论文将其重新表述为 **Seq2Seq 任务**，并提出了一个多层双向网络 (Multi-Layer Bidirectional Network，MLBiNet) 来 **融合跨句语义和关联事件信息，从而增强内各事件提及的判别**
  - 论文思路： 在解码事件标签向量序列时
    - 首先，为建模句子内部事件关系，我们提出双向解码器用于同时捕捉前向和后向事件依赖；
    - 然后，利用信息聚合器汇总句子语义和事件提及信息；
    - 最后，通过迭代多个由双向解码器和信息聚合器构造的单元，并在每一层传递邻近句子的汇总信息，最终感知到整个文档的语义和事件提及信息。

##### [【关于 知识图谱 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/)

- [【关于 知识图谱 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/)
  - 一、知识图谱简介
    - 1.1 引言
    - 1.2 什么是知识图谱呢？
      - 1.2.1 什么是图（Graph）呢？
      - 1.2.2 什么是 Schema 呢？
    - 1.3 知识图谱的类别有哪些？
    - 1.4 知识图谱的价值在哪呢？
  - 二、怎么构建知识图谱呢？
    - 2.1 知识图谱的数据来源于哪里？
    - 2.2 信息抽取的难点在哪里？
    - 2.3 构建知识图谱所涉及的技术？
    - 2.4、知识图谱的具体构建技术是什么？
      - 2.4.1 实体命名识别（Named Entity Recognition）
      - 2.4.2 关系抽取（Relation Extraction）
      - 2.4.3 实体统一（Entity Resolution）
      - 2.4.4 指代消解（Disambiguation）
  - 三、知识图谱怎么存储？
  - 四、知识图谱可以做什么？
- [爱奇艺知识图谱落地实践](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/爱奇艺知识图谱落地实践/)
  - 原文地址：[领域应用 | 完备的娱乐行业知识图谱库如何建成？爱奇艺知识图谱落地实践](https://mp.weixin.qq.com/s?__biz=MzU2NjAxNDYwMg==&mid=2247493658&idx=1&sn=cc2d7f82aa5c5a138dc7f267aaa26c16&chksm=fcb04fffcbc7c6e9575f5dcc3d1619425e4dd7fc0737976991bff687af6b1dadcdd20f906d04&mpshare=1&scene=22&srcid=0809aEdiDZ0DSoxjfzSF8Kcf&sharer_sharetime=1628471753625&sharer_shareid=da84f0d2d31380d783922b9e26cacfe2#rd)
  - 构建流程
    - 知识表示和建模：自顶向下的建模方式
    - 数据模式（schema）定义方式：
      - 基于 RDF(Resource Description Framework) 三元组
      - RDFS（RDF Schema） 的规则
    - 知识获取
      - 实体分类
        - 动机：主要**针对百度百科的数据**，因为**百度百科的数据没有类别信息**
        - 思路：
          - 构建基于规则池的分类器，生成训练数据，训练DNN模型（self-attention）文本分类模型；
          - DNN分类器与规则分类器互相扩充迭代（一到两轮），最终线上使用规则分类器。
      - 实体抽取
        - 目标：从数据中的识别和抽取实体的属性与关系信息
      - 知识融合
        - 流程：
          - 首先我们所有来源的实体数据都会进入原始实体库（RawEntity库），并且对原始表中的数据建立索引。
          - 当一个原始实体rawEntity入最终实体库之前，要在原始实体库中找是否有其它原始实体和rawEntity实际上是同一个实体。步骤：
            - 首先在索引中根据名字、别名等字段查询出若干个可能是相同实体的候选列表，这个步骤的目的是减少接下来流程的计算量。
            - 然后经过实体判别模型，根据模型得分识别出待合并对齐的原始实体；
            - 最后经过属性融合模型，将各原始实体的属性字段进行融合，生成最终的实体。
          - 这个流程中的合并判断模型实际上是通过机器学习训练生成的二分类器。
      - 知识存储

###### [【关于 实体链指篇】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/entity_linking/)
- [【关于  Low-resource Cross-lingual Entity Linking】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/entity_linking/LowResourceCrossLingualEntityLinking/)
  - 论文名称：Design Challenges in Low-resource Cross-lingual Entity Linking
  - 论文地址：https://arxiv.org/pdf/2005.00692.pdf
  - 来源：EMNLP 2020
- [【关于  GENRE】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/entity_linking/GENRE_ICLR21/)
  - 论文名称：AUTOREGRESSIVE ENTITY RETRIEVAL
  - 论文地址：https://openreview.net/pdf?id=5k8F6UU39V
  - 来源：ICLR 2021
  - 论文代码：https://github.com/facebookresearch/GENRE
  - 介绍：实体是我们表示和聚合知识的中心。例如，维基百科等百科全书是由实体构成的（例如，一篇维基百科文章）。检索给定查询的实体的能力是知识密集型任务（如实体链接和开放域问答）的基础。理解当前方法的一种方法是将分类器作为一个原子标签，每个实体一个。它们的权重向量是通过编码实体元信息（如它们的描述）产生的密集实体表示。
  - 缺点：
    - （i）上下文和实体的亲和力主要是通过向量点积来获取的，可能会丢失两者之间的细粒度交互；
    - （ii）在考虑大型实体集时，需要大量内存来存储密集表示；
    - （iii）必须在训练时对一组适当硬的负面数据进行二次抽样[。
  - 工作内容介绍：在这项工作中，我们提出了第一个 GENRE，通过生成其唯一的名称，从左到右，token-by-token 的自回归方式和条件的上下文。
  - 这使得我们能够缓解上述技术问题，
    - （i）自回归公式允许我们直接捕获文本和实体名称之间的关系，有效地交叉编码两者 ；
    - （ii）由于我们的编码器-解码器结构的参数随词汇表大小而不是词汇量大小而缩放，因此内存足迹大大减少实体计数；
    - （iii）准确的softmax损失可以有效地计算，而无需对负数据进行子采样。
  - 实验结果：我们展示了该方法的有效性，在实体消歧、端到端实体链接和文档检索任务上对20多个数据集进行了实验，在使用竞争系统内存占用的一小部分的情况下，获得了最新的或非常有竞争力的结果。他们的实体，我们只需简单地指定新的名称，就可以添加

###### [【关于 实体消歧 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/EntityDisambiguation/)

- [【关于 DeepType 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/EntityDisambiguation/DeepType/)
  - 论文：DeepType: Multilingual Entity Linking by Neural Type System Evolution
  - 论文地址：https://arxiv.org/abs/1802.01021
  - github：https://github.com/openai/deeptype

###### [【关于KGQA 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/KGQA/)

- [【关于KGQA 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/KGQA/)
  - 一、基于词典和规则的方法
  - 二、基于信息抽取的方法
- [【关于 Multi-hopComplexKBQA 】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/KGQA/ACL20_Multi-hopComplexKBQA/)
  - 论文：Lan Y, Jiang J. Query Graph Generation for Answering Multi-hop Complex Questions from Knowledge Bases[C]//Proceedings of the 58th Annual Meeting of the Association for Computational Linguistics. 2020: 969-974.
  - 会议：ACL2020
  - 链接：https://www.aclweb.org/anthology/2020.acl-main.91/
  - 代码：https://github.com/lanyunshi/Multi-hopComplexKBQA

###### [【关于Neo4j  】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/neo4j/)

- [【关于Neo4j】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/neo4j/)
  - 一、Neo4J 介绍与安装
    - 1.1 引言
    - 1.2 Neo4J 怎么下载？
    - 1.3 Neo4J 怎么安装？
    - 1.4 Neo4J Web 界面 介绍
    - 1.5 Cypher查询语言是什么？
  - 二、Neo4J 增删查改篇
    - 2.1 引言
    - 2.2 Neo4j 怎么创建节点？
    - 2.3 Neo4j 怎么创建关系？
    - 2.4 Neo4j 怎么创建 出生地关系？
    - 2.5 Neo4j 怎么查询？
    - 2.6 Neo4j 怎么删除和修改？
  - 三、如何利用 Python 操作 Neo4j 图数据库？
    - 3.1 neo4j模块：执行CQL ( cypher ) 语句是什么？
    - 3.2 py2neo模块是什么？
  - 四、数据导入 Neo4j 图数据库篇

- [【关于 Neo4j 索引】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/KG_study/neo4j/index.md)

##### [【关于 细粒度情感分析】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/ABSC_study/)

- [【关于 LCF】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/ABSC_study/LCF/)
  - 论文名称：A Local Context Focus Mechanism for Aspect-Based Sentiment Classiﬁcation
  - 论文动机：没有考虑情感极性和局部上下文间关系
    - LCF:利用自注意力机制同时捕获局部上下文特征和全局上下文特征，以推断 targeted aspect 的情感极性
    - SRD:评估上下文词与 aspect 间的独立性，SRD对于弄清局部上下文具有重要意义，并且SRD阈值中的上下文单词的特征将得到保留和重点关注。
    - CDM 和 CDW 层：强化 LCF，使其对 特殊 aspest 的局部上下文提供 更多 注意力。CDM层通过掩盖语义相对较少的上下文词的输出表示，将重点放在局部上下文上。 CDW 层根据 SRD 削弱语义相对较少的上下文词的特征；
  
##### [【关于 主动学习】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/active_learn_study/)

- [【关于 Proactive Learning for Named Entity Recognition（命名实体识别的主动学习）】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/active_learn_study/ProactiveLearningforNamedEntityRecognition/)

##### [【关于 对抗训练】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/adversarial_training_study/)

- [【关于 生成对抗网络 GAN 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DL_algorithm/adversarial_training_study/)
- [【关于 FreeLB 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/adversarial_training_study/FREELB/)
  - 论文名称: FreeLB: Enhanced Adversarial Training for Language Understanding 加强语言理解的对抗性训练
  - 动机：对抗训练使保留标签的输入扰动的最大风险最小，对于提高语言模型的泛化能力是有效的。 
  - 方法：提出了一种新的对抗性训练算法—— freeb，它通过在字嵌入中添加对抗性的干扰，最小化输入样本周围不同区域内的对抗性风险，从而提高嵌入空间的鲁棒性和不变性。

##### [【关于 GCN in NLP 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/GNN/GCN2NLP/)
- [【关于 GCN in NLP 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/GNN/GCN2NLP/readme.md)
  - 构图方法：
    - 句法依赖树；
    - TF-IDF;
    -  PMI;
    -  序列关系；
    -  词典
 
##### [【关于 文本预处理】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/NLP_tools/pre_study/samplingStudy/)
- [【关于 过采样】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/NLP_tools/pre_study/samplingStudy/samplingStudy)

##### [【关于问答系统】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/) 

- [【关于 FAQ Trick】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/FAQ/FAQ_trick/)
- [【关于 文本匹配和多轮检索】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/文本匹配和多轮检索.xmind)
- [【关于 FAQ】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/FAQ/)
  - [【关于 LCNQA】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/LCNQA/)
    - 论文名称：Lattice CNNs for Matching Based Chinese Question Answering
  - [LSTM-based Deep Learning Models for Non-factoid Answer Selection](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/T1_LSTM-based_for_Non-factoid_Answer_Selection/)
  - [【关于 Denoising Distantly Supervised ODQA】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/T4_DenoisingDistantlySupervisedODQA/)
    - 论文名称：Denoising Distantly Supervised Open-Domain Question Answering
  - [FAQ retrieval using query-question similarity and BERT-based query-answer relevance](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/ACM2019_faq_bert-based_query-answer_relevance/)
  - [【DC-BERT】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/SIGIR2020_DCBert/)
    - 论文名称：DC-BERT : DECOUPLING QUESTION AND DOCUMENT FOR EFFICIENT CONTEXTUAL ENCODING
- [【关于 KBFAQ】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/KBFAQ/)
- [【关于 MulFAQ】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/mulFAQ/)
  - [【关于 MSN】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/mulFAQ/MSN_mulQA/)
    - 论文名称：Multi-hop Selector Network for Multi-turn Response Selection in Retrieval-based chatbots
    - 论文地址：https://www.aclweb.org/anthology/D19-1011.pdf
    - 论文项目：https://github.com/chunyuanY/Dialogue
    - 动机：
      - 1. 上下文拼接问题：将候选回复与上下文utterance在多粒度级别进行匹配，这种方式忽略了使用过多的上下文信息带来副作用。
      - 2. 根据直接，一般来说距离回复越近的utterance，越能够反应最终轮对话的意图。所以，我们首先使用最后一个utterance作为key去选择word级别和sentence级别上相关的上下文回复。然而，我们发现**许多样本中最后一个utterance都是一些短句并且很多都是无效信息**（比如good, ok）
    - 方法：提出一种多跳选择网络（multi-hop selector network, MSN）
      - s1 ：采用 多跳选择器从 上下文集 中 选取最相关的上下文 utterances，并生成 k 个 不同的上下文；
      - s2 : 融合 k 个 上下文 utterance ，并与候选回复做匹配；
      - s3 : 匹配截取，采用 CNN 提取匹配特征，并 用 GRU 学习 utterance 间的临时关系；

##### [【关于 文本摘要】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/summarization_study/) 

- [【关于 Bertsum】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/summarization_study/EMNLP2019_bertsum/) **【推荐阅读】**
  - 论文名称：Fine-tune BERT for Extractive Summarization
  - 会议：EMNLP2019
  - Bert 在抽取式文本摘要中的应用
    - 问题：
      - 如何获得每个句子向量？
      - 如何将向量用于二分类问题？
      - 如何判断每个句子的去留？
  - 思路：定义文档 $d=[sent_1,sent_2,...,sent_m]$,$sent_i$ 表示 文档中的第$i$个句子，Extractive summarization 定义为 给每个$sent_i$分配一个标签$y_i∈{0,1}$，用于判断该句子是否包含于 摘要 中。
    - 方法介绍
      - Extractive Summarization with BERT
        - 动机：
          - Bert 作为 一个 masked-language model，输出向量基于标记而不是句子；
          - Bert 只包含 两个标签（sentence A or sentence B），而不是多个句子；
        - 方法
          - Encoding Multiple Sentences：在每个句子之前插入一个[CLS] token**【bert 就开头一个】**，在每个句子之后插入一个[SEP] token 
          - Interval Segment Embeddings 
            - 我们使用区间段嵌入来区分文档中的多个句子。
  
> 例如：对于$[sent_1，sent_2，sent_3，sent_4，sent_5]$，我们将分配[E_A，E_B，E_A，E_B，E_A]
> $sent_i$ 由向量 $T_i$ 表示，$T_i$是来自顶部BERT层的第$i$个[CLS]符号的向量。

- [【关于Pointer-Generator Networks 指针网络】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/summarization_study/ACL2017_Pointer_Generator_Networks/)
  - 论文名称：Get To The Point: Summarization with Pointer-Generator Networks
  - 会议：ACL2017
  - 动机：
    - 文本摘要类别
      - extractive 抽取式
        - 方式：直接从原文抽取一些段落
        - 优点：简单
        - 问题：无法生成高质量的摘要，因为不具备一些复杂的摘要能力(如释义(paraphasing), 概括(generalization), 与现实世界知识的融合(incorporation of real-world knowledge))
      - abstractive 生成式
        - 方式：根据长文本 生成 摘要
        - 代表：seq2sq架构
        - 问题：
          - 难以准确复述原文细节；
          - 无法处理原文中的未登录词(OOV)；
          - 在生成的摘要中存在一些重复的部分；
  - 方法：
    - 编码器（encoder） 
      - 方式：BiLSTM
      - 作用：将文章中每个词的词向量编码为 隐状态 ht
    - 解码器（decoder）
      - 方式：单向 LSTM
      - 作用：每一时刻 t，将上一时刻 生成 的 词的词向量作为输入，得到 Decoder Hidden State st，该状态被用于计算attention分布和词的预测
    - Attention
      - 作用：每个时间步t,考虑当前序列的注意力分布，注意力分布用于生成编码器隐藏状态的加权总和，转化为上下文向量，与解码器t时刻的隐状态进行concatenated然后喂到两个线性层来计算词汇分布P（一个固定维度的向量，每个维度代表被预测词的概率，取argmax就能得到预测的单词）。
      - 目的：告诉模型在当前步的预测过程中，原文中的哪些词更重要

##### [【关于 文本匹配】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/) 

- [【关于 /SimCSE】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/SimCSE/) **【推荐阅读】**
  - 论文：SimCSE: Simple Contrastive Learning of Sentence Embeddings
  - 会议：
  - 论文地址：https://arxiv.org/abs/2104.08821
  - 论文代码：https://github.com/princeton-nlp/SimCSE
  - 思路：
    - 首先描述了一种无监督方法，它采用输入句子并在对比目标中预测自己，仅将标准 dropout 用作噪声。这种简单的方法效果出奇地好，与以前的受监督计数器部件相当。我们假设 dropout 充当最小数据增强的大小，删除它会导致表示崩溃。
    - 然后，我们从最近从自然语言推理 (NLI) 数据集中学习句子嵌入的成功中汲取灵感，并将 NLI 数据集中的注释对合并到对比学习中，方法是使用“蕴含”对作为正例，将“矛盾”对作为硬负例。
  - 实验结果：
    - 作者评估了标准语义文本相似性（STS）任务上的 SimCSE，使用 BERT-base 的无监督和监督模型分别平均实现了 74.5％ 和 81.6％ 的 Spearman 相关性，与之前的最佳结果相比，分别提高了 7.9 和 4.6点。
    - 作者还表明，对比学习理论上将嵌入分布得更均匀，并且在有监督信号可用时，它可以更好地对齐正样本。
- [【关于 BERT-flow 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/BERTFlow/)
  - 论文：On the Sentence Embeddings from Pre-trained Language Models
  - 会议：EMNLP2020
  - 论文地址：https://arxiv.org/pdf/2011.05864.pdf
  - 论文代码：https://github.com/bohanli/BERT-flow
  - 前沿：像BERT这样的经过预训练的上下文表示在自然语言处理中取得了巨大的成功；
  - 动机：已经发现，未经微调的来自预训练语言模型的句子嵌入很难捕获句子的语义；
  - 论文方法：在本文中，我们认为BERT嵌入中的语义信息没有得到充分利用。我们首先从理论上揭示了掩盖的语言模型预训练目标与语义相似性任务之间的理论联系，然后从经验上分析了BERT句子的嵌入。
  - 实验结果：我们发现BERT总是诱发非光滑的各向异性语义空间，这会损害其语义相似性的表现。为解决此问题，我们建议通过将非正则化的流量标准化来将各向异性的语义嵌入分布转换为平滑的各向异性高斯分布。实验结果表明，我们提出的BERT流方法在各种语义文本相似性任务上比最先进的句子嵌入方法具有明显的性能提升。
- [【关于 Sentence-BERT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/sentence_bert/)
  - 项目地址：https://github.com/km1994/nlp_paper_study
  - 论文：Sentence-BERT: Sentence Embeddings using Siamese BERT-Networks
  - github:https://github.com/UKPLab/sentence-transformers
  - 动机：
    - 方法一：BERT使用交叉编码器：将两个句子传递到变压器网络，并预测目标值；
      - 问题： 由于太多可能的组合，此设置不适用于各种对回归任务。 在n = 10000个句子的集合中找到相似度最高的对需要BERT n·（n-1）/ 2 = 49 995 000推理计算。 在现代V100 GPU上，这大约需要65个小时。 类似地，对于一个新问题，找到Quora的超过4,000万个现有问题中最相似的一个可以建模为与BERT的成对比较，但是，回答单个查询将需要50多个小时。
    - 方法二：解决聚类和语义搜索的常用方法是将每个句子映射到向量空间，以使语义相似的句子接近。 研究人员已开始将单个句子输入BERT，并得出固定大小的句子嵌入。 最常用的方法是平均BERT输出层（称为BERT嵌入）或通过使用第一个令牌的输出（[CLS]令牌）；
      - 问题：就像我们将要展示的那样，这种常规做法产生的句子嵌入效果很差，通常比平均GloVe嵌入效果更差。
  - 论文方法：
    - 我们开发了SBERT。 siamese network 体系结构使得可以导出输入句子的固定大小矢量。 使用余弦相似度或Manhatten / Euclidean距离之类的相似度度量，可以找到语义上相似的句子。 
  - 存在问题解答：
    - 小问题：[在语义相似度任务中，SBERT的计算速度为什么比纯bert进行句子编码要快？](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/sentence_bert/)
- [【关于 语义相似度匹配任务中的 BERT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/bert_similairity/)  **【推荐阅读】**
  - 阅读理由：BERT 在 语义相似度匹配任务 中的应用，可以由很多种方式，然而，你真的了解这些方式的区别和优缺点么？
  - 动机：BERT 在 语义相似度匹配任务 中的应用，可以常用 Sentence Pair Classification Task：使用 [CLS]、cosine similairity、sentence/word embedding、siamese network 方法，那么哪种是最佳的方式呢？你是否考虑过呢?
- [【关于 MPCNN】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/Multi-PerspectiveSentenceSimilarityModelingwithCNN/)
  - 论文：Multi-Perspective Sentence Similarity Modeling with Convolution Neural Networks
- [【关于 RE2】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/Multi-RE2_study/)
  - 论文：Simple and Effective Text Matching with Richer Alignment Features
  - 动机： 可以使用多个序列间比对层构建更强大的模型。 代替基于单个对准过程的比较结果进行预测，具有多个对准层的堆叠模型将保持其中间状态并逐渐完善其预测。**但是，由于底层特征的传播效率低下和梯度消失，这些更深的体系结构更难训练。** 
  - 介绍：一种快速强大的神经体系结构，具有用于通用文本匹配的多个对齐过程。 我们对以前文献中介绍的文本匹配方法中许多慢速组件的必要性提出了质疑，包括复杂的多向对齐机制，对齐结果的大量提炼，外部句法特征或当模型深入时用于连接堆叠块的密集连接。 这些设计选择会极大地减慢模型的速度，并且可以用重量更轻且效果相同的模型代替。 同时，我们重点介绍了有效文本匹配模型的三个关键组成部分。 这些组件（名称为RE2代表）是以前的对齐特征（残差矢量），原始点向特征（嵌入矢量）和上下文特征（编码矢量）。 其余组件可能尽可能简单，以保持模型快速，同时仍能产生出色的性能。
- [【关于 DSSM】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/cikm2013_DSSM/)
  - 论文：Deep Structured Semantic Model
  - 论文会议：CIKM2013
  - 问题：语义相似度问题
    - 字面匹配体现
      - 召回：在召回时，传统的文本相似性如 BM25，无法有效发现语义类 Query-Doc 结果对，如"从北京到上海的机票"与"携程网"的相似性、"快递软件"与"菜鸟裹裹"的相似性
      - 排序：在排序时，一些细微的语言变化往往带来巨大的语义变化，如"小宝宝生病怎么办"和"狗宝宝生病怎么办"、"深度学习"和"学习深度"；
    - 使用 LSA 类模型进行语义匹配，但是效果不好
  - 思路：
    - 利用 表示层 将 Query 和 Title 表达为低维语义向量；
    - 通过 cosine 距离来计算两个语义向量的距离，最终训练出语义相似度模型。
  - 优点
    - 减少切词的依赖：解决了LSA、LDA、Autoencoder等方法存在的一个最大的问题，因为在英文单词中，词的数量可能是没有限制，但是字母 n-gram 的数量通常是有限的
    - 基于词的特征表示比较难处理新词，字母的 n-gram可以有效表示，鲁棒性较强；
    - 传统的输入层是用 Embedding 的方式（如 Word2Vec 的词向量）或者主题模型的方式（如 LDA 的主题向量）来直接做词的映射，再把各个词的向量累加或者拼接起来，由于 Word2Vec 和 LDA 都是无监督的训练，这样会给整个模型引入误差，DSSM 采用统一的有监督训练，不需要在中间过程做无监督模型的映射，因此精准度会比较高；
    - 省去了人工的特征工程；
  - 缺点
    - word hashing可能造成冲突
    - DSSM采用了词袋模型，损失了上下文信息
    - 在排序中，搜索引擎的排序由多种因素决定，由于用户点击时doc的排名越靠前，点击的概率就越大，如果仅仅用点击来判断是否为正负样本，噪声比较大，难以收敛
- [【关于 ABCNN 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/TACL2016_ABCNN/)
  - 论文：ABCNN: Attention-Based Convolutional Neural Network for Modeling Sentence Pairs
  - 会议：TACL 2016
  - 论文方法：采用了CNN的结构来提取特征，并用attention机制进行进一步的特征处理，作者一共提出了三种attention的建模方法
- [【关于 ESIM 】那些你不知道的事 ](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/TACL2017_ESIM/)
  - 论文：Enhanced LSTM for Natural Language Inference
  - 会议：TACL2017
  - 自然语言推理（NLI: natural language inference）问题：
    - 即判断能否从一个前提p中推导出假设h
    - 简单来说，就是判断给定两个句子的三种关系：蕴含、矛盾或无关
  - 论文方法：
    - 模型结构图分为左右两边：
    - 左侧就是 ESIM，
    - 右侧是基于句法树的 tree-LSTM，两者合在一起交 HIM (Hybrid Inference Model)。
    - 整个模型从下往上看，分为三部分：
      - input encoding；
      - local inference modeling；
      - inference composition；
      - Prediction
- [【关于 BiMPM 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/IJCAI2017_BiMPM/)
  - 论文：Bilateral multi-perspective matching for natural language sentences
  - 会议：IJCAI2017
  - 方法：
    - Word Representation Layer:其中词表示层使用预训练的Glove或Word2Vec词向量表示, 论文中还将每个单词中的字符喂给一个LSTM得到字符级别的字嵌入表示, 文中使用两者构造了一个dd维的词向量表示, 于是两个句子可以分别表示为 P:[p1,⋯,pm],Q:[q1,⋯,qn].
    - Context Representation Layer: 上下文表示层, 使用相同的双向LSTM来对两个句子进行编码. 分别得到两个句子每个时间步的输出.
    - Matching layer: 对两个句子PP和QQ从两个方向进行匹配, 其中⊗⊗表示某个句子的某个时间步的输出对另一个句子所有时间步的输出进行匹配的结果. 最终匹配的结果还是代表两个句子的匹配向量序列.
    - Aggregation Layer: 使用另一个双向LSTM模型, 将两个匹配向量序列两个方向的最后一个时间步的表示(共4个)进行拼接, 得到两个句子的聚合表示.
- Prediction Layer: 对拼接后的表示, 使用全连接层, 再进行softmax得到最终每个标签的概率.
- [【关于 DIIN 】那些你不知道的事 ](https://github.com/km1994/nlp_paper_study/tree/master/text_match_study/T2017_DIIN/)
  - 论文：Densely Interactive Inference Network
  - 会议：TACL2017
  - 模型主要包括五层：嵌入层（Embedding Layer）、编码层（Encoding Layer）、交互层（Interaction Layer ）、特征提取层（Feature Extraction Layer）和输出层（Output Layer）
- [【关于 DC-BERT】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/SIGIR2020_DCBert/)
  - 论文名称：DC-BERT : DECOUPLING QUESTION AND DOCUMENT FOR EFFICIENT CONTEXTUAL ENCODING
  - 阅读理由：Bert 在 QA 上面的应用
  - 动机：Bert 无法处理传入问题的高吞吐量，每个问题都有大量检索到的文档；
  - 论文方法：具有双重BERT模型的解耦上下文编码框架：
    - 一个在线BERT，仅对问题进行一次编码；
    - 一个正式的BERT，对所有文档进行预编码并缓存其编码；
- [【关于 tBERT 】那些你不知道的事 ](https://github.com/km1994/nlp_paper_study/tree/master/QA_study/SIGIR2020_DCBert/)
   - 论文：tBERT: Topic Models and BERT Joining Forces for Semantic Similarity Detection
   - 会议：ACL2020
   - 论文地址：https://www.aclweb.org/anthology/2020.acl-main.630/
   - 论文代码：https://github.com/wuningxi/tBERT
   - 动机：未存在将主题模型和BERT结合的方法。 语义相似度检测是自然语言的一项基本任务理解。添加主题信息对于以前的特征工程语义相似性模型和神经网络模型都是有用的其他任务。在那里目前还没有标准的方法将主题与预先训练的内容表示结合起来比如 BERT。
   - 方法：我们提出了一种新颖的基于主题的基于BERT的语义相似度检测体系结构，并证明了我们的模型在不同的英语语言数据集上的性能优于强神经基线。我们发现在BERT中添加主题特别有助于解决特定领域的情况。




##### [【关于 机器翻译】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/MachineTranslation/)

- [Neural Machine Translation of Rare Words with Subword Units 论文学习](https://github.com/km1994/nlp_paper_study/tree/master/MachineTranslation/NeuralMachineTranslationOfRareWordsWithSubwordUnits/)

##### [【关于 文本生成】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_generation/)

- [【关于 SLCVAE 安装 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_generation/SLCVAE/)
- [【关于 ScriptWriter 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_generation/ScriptWriter/)
  - 论文：ScriptWriter: Narrative-Guided Script Generation
  - 发表会议：ACL2020
  - 论文地址：https://arxiv.org/abs/2005.10331
  - github：https://github.com/DaoD/ScriptWriter
  - 论文动机：如果人为提供一些参考信息（例如情节），能否进一步提高文本生成的质量？例如，在故事生成这一问题中，现有模型要从头考虑如何生成一整个故事，难度比较大，那如果人为提供一个故事线，是否可以提升模型的性能呢？
  - 论文方法：
    - 根据给定的情节和已有的台词上文生成后续台词。在这一模型中，我们设计了一个情节追踪模块，这一模块可以使模型根据已有的上文内容判断情节的表达情况，并在后续生成中更加关注未表达的情节。实验结果表明，情节的确可以帮助模型提高台词的生成质量，且相比于其他模型，ScriptWriter能够更有效地利用情节信息。
  - 论文思路：
  1. 多层注意力机制：将情节、上文、候选回复表示为向量。
  2. 情节更新机制：使情节的表示包含更多未表达部分的情节信息。
  3. 抽取了三类匹配特征：
     1. （1）上文-回复匹配，其能够反映回复是否与上文连贯；
     2. （2）情节-回复匹配，其能够反映回复是否与情节相符；
     3. （3）上文-情节匹配，其能够隐式反映哪些情节已经被上文表达。
  4. 最后，这些匹配特征经过CNN的进一步抽取和聚集，再经过MLP得到最终的匹配得分。

##### [【关于 对话系统】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/)

- [【关于 Domain/Intent Classification 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/IntentClassification/)
- [【关于 槽位填充 (Slot Filling)】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/SlotFilling/)
- [【关于 上下文LU】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/contextLU/)
- [【关于 DSTC 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/DSTC/)

###### [【关于 自然语言生成NLG 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/NLG/)
- [【关于 自然语言生成NLG 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/NLG/)
- [【关于 IRN 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/NLG/IRN/)
  - 论文：ScriptWriter: Narrative-Guided Script Generation
  - 发表会议：ACL2020
  - 论文地址：https://www.aclweb.org/anthology/2020.acl-main.10/
  - github：#
  - 论文动机：如何将输入中对话状态的slot-value对正确的在response生成
  - 论文方法：
    - 迭代网络：来不断修正生成过程不对的slot-value；
    - 强化学习：不断更新，实验证明我们的网络生成的回复中中slot关键信息生成的正确性大大提高。
  - 实验结果：对多个基准数据集进行了综合研究，结果表明所提出的方法显著降低了所有强基线的时隙错误率。人类的评估也证实了它的有效性。

###### [【关于 E2E 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/E2E/)

- [【关于 TC_Bot(End-to-End Task-Completion Neural Dialogue Systems) 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/E2E/TC_Bot/)
- [【关于 DF-Net 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/E2E/DynamicFusionNetwork/)
  - 论文：Dynamic Fusion Network for Multi-Domain End-to-end Task-Oriented Dialog
  - 发表会议：ACL2020
  - 论文地址：https://arxiv.org/abs/2004.11019
  - github：https://github.com/LooperXX/DF-Netmd
  - 论文动机：
    1. 依赖大量标准数据：端到端的模型依赖于大量的标注数据，这就导致了模型在一个新拓展的领域上很难利用。
    2. 对于一个新的领域，总是很难收集足够多的数据。这就使得将知识从具有充足标注数据的源领域迁移到一个只有少量标注数据的新领域成为非常重要的问题。
  - 前沿工作总结
    - 第一类：简单地结合多领域的数据集进行训练，如图 (a)
      - 优点：隐含地提取共享的特征
      - 缺点：很难有效捕捉领域特有的知识
    - 第二类是在各个领域单独地训练模型，如图 (b)
      - 优点：能够很好地捕捉领域特有的知识；
      - 缺点：却忽视了不同领域间共有的知识。
    - 第三类：通过建模不同领域间知识的连接来解决已有方法的局限。已有的一个简单的baseline如图 (c)，将领域共享的和领域私有的特征合并在一个共享-私有 (shared-private) 架构中。
      - 优点：区分了共享以及私有的知识
      - 缺点：
        - 一是面对一个几乎不具备数据的新领域时，私有模块无法有效提取对应的领域知识；
        - 二是这个架构忽略了一些领域子集间细粒度的想关性（比如和天气领域相比，导航领域和规划领域更相关）。
  - 思路：
  1. shared-private 架构：学习共享的知识以及对应的领域特有特征；
  2. 动态融合网络：动态地利用所有领域间的相关性提供给下一步细粒度知识迁移；
  3. 对抗训练 (adversarial training) ：促使共享模块生成领域共享特征

##### [【关于 Rasa 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/)

1. [【关于 rasa 安装 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa安装手册.md)
2. [【关于 rasa 基本架构 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa基本框架_视频讲解.md)
3. [【关于 rasa中文对话系统】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa中文对话系统.md)
4. [【关于 rasa中文对话系统构建】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa中文对话系统构建.md)
5. [【关于 rasa->NLU 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa系列/rasa_nlu.md)
6. [【关于 rasa -> Core -> FormAction 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa_core_FormAction/rasa_nlu.md)
7. [【关于 rasa -> Core -> Stories 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa系列/rasa_core_Stories.md)
8. [【关于 rasa -> Core -> Action 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/DialogueSystem_study/rasa/rasa_core_FormAction/rasa_core_Action.md)

##### [【关于 半监督学习】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/Unsupervised/)

- [Unsupervised Data Augmentation (UDA)](https://github.com/km1994/nlp_paper_study/tree/master/Unsupervised/UDA/)
  - [【关于 UDA】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/Unsupervised/UDA/)
    - 阅读理由：UDA（Unsupervised Data Augmentation 无监督数据增强）是Google在2019年提出的半监督学习算法。该算法超越了所有现有的半监督学习方法，并实现了仅使用极少量标记样本即可达到使用大量标记样本训练集的精度。
    - 动机： 深度学习的模型训练通常依赖大量的标签数据，在只有少量数据上通常表现不好;
    - 思路：提出了一种基于无监督数据的数据增强方式UDA（Unsupervised Data Augmentation）。UDA方法生成无监督数据与原始无监督数据具备分布的一致性，而以前的方法通常只是应用高斯噪声和dropout噪声（无法保证一致性）。UDA方法利用了一种目前为止最优的方法生成更加“真实”的数据。
    - 优点：使用这种数据增强方法，在极少量数据集上，六种语言任务和三种视觉任务都得到了明显的提升。
- [【关于 “脏数据”处理】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/Unsupervised/noisy_label_learning/)
  -  一、动机
     - 1.1 何为“脏数据”？
     - 1.2 “脏数据” 会带来什么后果？
   - 二、“脏数据” 处理篇
     - 2.1 “脏数据” 怎么处理呢？
     - 2.2 置信学习方法篇
       - 2.2.1 什么是 置信学习方法？
       - 2.2.2 置信学习方法 优点？
       - 2.2.3 置信学习方法 怎么做？
       - 2.2.4 置信学习方法 怎么用？有什么开源框架？
       - 2.2.5 置信学习方法 的工作原理？

##### [【关于 NLP分类任务】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/classifier_study/)

- [【关于 NLP分类任务】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/classifier_study/) 
  - 转载于：JayLou娄杰大佬的 [如何解决NLP分类任务的11个关键问题：类别不平衡&低耗时计算&小样本&鲁棒性&测试检验&长文本分类](https://zhuanlan.zhihu.com/p/183852900)
- [【关于 文本分类 trick】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/classifier_study/classifier_trick/)
  - 一、数据预处理篇
    - 1.1 vocab 构建问题
    - 1.2 模型输入问题
    - 1.3 噪声数据处理问题
    - 1.4 中文任务分词问题
    - 1.5 停用词处理问题
  - 二、模型篇
    - 2.1 模型选择问题
    - 2.2 词袋模型 or 词向量————词向量选择问题
    - 2.3 字 or 词向量———— 粒度选择问题
  - 三、参数篇
    - 3.1 正则化问题
    - 3.2 学习率问题
  - 四、任务篇
    - 4.1 二分类问题
    - 4.2 多标签分类问题
    - 4.3 长文本问题
    - 4.4 鲁棒性问题
  - 五、标签体系构建
    - 5.1 标签体系构建问题
    - 5.2 标签体系合理性评估问题
  - 六、策略构建篇
    - 6.1 算法策略构建问题
    - 6.2 特征挖掘策略问题
    - 6.3 数据不均衡问题
      - 6.3.1 重采样（re-sampling）
      - 6.3.2 重加权（re-weighting）
      - 6.3.3 数据增强
    - 6.4 预训练模型融合角度问题
    - 6.5 灾难性遗忘问题
    - 6.6 小模型大智慧
      - 6.6.1 模型蒸馏
      - 6.6.2 数据蒸馏
- [【关于 Knowledge in TextCNN】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/classifier_study/KG_classifier/)
  - 论文： Combining Knowledge with Deep Convolutional Neural Networks for Short Text Classification
  - github：https://zhuanlan.zhihu.com/p/183852900
  - 介绍：文本分类是NLP应用程序中的一项基本任务。 现有的大多数工作都依靠显式或隐式文本表示来解决此问题。 
  - 问题：虽然这些技术对句子很有效，但由于其简短和稀疏，因此无法轻松地应用于短文本。
  - 方法：提出了一个基于卷积神经网络的框架，该框架结合了短文本的显式和隐式表示形式进行分类
    - 首先使用大型分类学知识库将短文本概念化为一组相关概念。 
    - 然后，通过在预训练的单词向量之上合并单词和相关概念来获得短文本的嵌入。 
    - 我们进一步将字符级功能集成到模型中，以捕获细粒度的子词信息。 
  - 实验结果：在五个常用数据集上的实验结果表明，我们提出的方法明显优于最新方法。
- [【关于 LOTClass】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/classifier_study/LOTClass/)
  - 论文名称：《Text Classification Using Label Names Only: A Language Model Self-Training Approach》
  - 会议：EMNLP2020
  - 论文地址：https://arxiv.org/pdf/2010.07245.pdf
  - 论文源码地址：https://github.com/yumeng5/LOTClass
  - 动机
    - 监督学习：标注数据昂贵
    - 半监督学习：虽然减少了对标注数据的依赖，但还是需要领域专家手动进行标注，特别是在类别数目很大的情况下
    - 关键词积累：关键词在不同上下文中也会代表不同类别
  - 方法：
    - 提出了一种基于预训练神经 LM 的弱监督文本分类模型 LotClass，它不需要任何标记文档，只需要每个类的标签名称。
    - 提出了一种寻找类别指示词的方法和一个基于上下文的单词类别预测任务，该任务训练LM使用一个词的上下文来预测一个词的隐含类别。经过训练的LM很好地推广了基于未标记语料库的自训练文档级分类
  - 在四个分类数据集上，LOTClass明显优于各弱监督模型，并具有与强半监督和监督模型相当的性能。

- [【关于 PET 】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/classifier_study/PET/)
  - 论文名称：《exploiting cloze questions for few shot text classification and natural language inference 》
  - 会议：EMNLP2020
  - 论文地址：chrome-extension://ikhdkkncnoglghljlkmcimlnlhkeamad/pdf-viewer/web/viewer.html?file=https%3A%2F%2Faclanthology.org%2F2021.eacl-main.20.pdf#=&zoom=125
  - 论文源码地址：https://github.com/timoschick/pet

##### [【关于 中文分词】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/chinese_word_segmentation/)

- [【关于 中文分词】那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/chinese_word_segmentation/)
  - 一、什么是 中文分词？
  - 二、为什么用使用 中文分词，直接用句子或字不好么？
  - 三、中文分词 有哪些难点？
  - 四、常用方法有哪些？
    - 4.1 基于词典的中文分词方法
      - 4.1.1 正向最大匹配法
      - 4.1.2 负向最大匹配法
      - 4.1.3 双向最大匹配法
    - 4.2 基于N-gram语言模型的分词方法
    - 4.3 基于规则的中文分词方法
- [【关于 DAAT 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/chinese_word_segmentation/DAAT/)
  - 论文：Coupling Distant Annotation and Adversarial Training for Cross-Domain Chinese Word Segmentation
  - 发表会议：ACL2020
  - 论文地址：hhttps://arxiv.org/abs/2007.08186
  - github：https://github.com/Alibaba-NLP/DAAT-CWS
  - 动机：完全监督的神经方法在中文分词（CWS）的任务中取得了重大进展。将监督模型应用于域外数据时，其性能往往会急剧下降。
    - 性能下降原因：
      - 跨域的分布差距
      - 词汇不足（OOV）问题
  - 方法
    - Distant annotation（DA）
      - 目的：自动生成目标域内句子的分词结果
      - 方法：是在不需要任何人工定义词典的情况下，自动对目标领域文本实现自动标注。
      - 思路：
        - 基本分词器：使用来自源域的标注数据训练，用于识别源域和目标域中常见的单词
        - 特定领域的单词挖掘器：旨在探索目标特定于领域的单词
      - 存在问题
        - 存在影响最终性能的标注错误问题
    - Adversarial Training（AT）
      - 动机：为了降低噪声数据的影响，更好地利用源域数据，
      - 方法：在源域数据集和通过Distant annotation构造的目标领域数据集上联合进行Adversarial training的方法。
      - 优点：Adversarial training模块可以捕获特定领域更深入的特性，和不可知领域的特性。

##### [【关于 关键词提取】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/keyword_ex_study/)

- [【关于 关键词提取】 那些你不知道的事](keyword_ex_study/)
  - 一、TF-IDF关键词提取算法
    - 1.1 理论基础
    - 1.2 计算公式
      - 1.2.1 词频 （Term Frequency，TF）
      - 1.2.2 逆文本频率(Inverse Document Frequency，IDF)
      - 1.2.3 TF-IDF
    - 1.3 应用
    - 1.4 实战篇
      - 1.4.1 TF-IDF算法 手撸版
      - 1.4.2 TF-IDF算法 Sklearn 版
      - 1.4.3 TF-IDF算法 jieba 版
  - 二、PageRank算法【1】
    - 2.1 理论学习
  - 三、TextRank算法【2】
    - 3.1 理论学习
    - 3.2 实战篇
      - 3.2.1 基于Textrank4zh的TextRank算法版
      - 3.2.2 基于jieba的TextRank算法实现
      - 3.2.3 基于SnowNLP的TextRank算法实现
- [【关于 KeyBERT 】 那些你不知道的事](keyword_ex_study/KeyBert/)
  - 论文：Sharma, P., & Li, Y. (2019). Self-Supervised Contextual Keyword and Keyphrase Retrieval with Self-Labelling.
  - 论文地址：https://www.preprints.org/manuscript/201908.0073/download/final_file
  - 论文代码：https://github.com/MaartenGr/KeyBERT
  - 一、摘要
  - 二、动机
  - 三、论文方法
  - 四、实践
    - 4.1 安装
    - 4.2 KeyBERT 调用
    - 4.3 语料预处理
    - 4.4 利用 KeyBert 进行关键词提取

##### [【关于 搜索引擎】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/search_engine/)

- [【关于 搜索引擎】 那些你不知道的事](search_engine/)
  - [搜索系统的架构设计](#搜索系统的架构设计)
    - [搜索 QP（query理解）的架构设计](#搜索-qpquery理解的架构设计)
  - [搜索j介绍](#搜索j介绍)
    - [搜索排序 介绍](#搜索排序-介绍)
    - [Embedding 搜索](#embedding-搜索)
      - [动机](#动机)
      - [Embedding 搜索优点](#embedding-搜索优点)
      - [Embedding的学习形式](#embedding的学习形式)
      - [Embedding 搜索 所关心的问题](#embedding-搜索-所关心的问题)
      - [参考资料](#参考资料)
    - [Query纠错](#query纠错)
      - [Query纠错 之  原理](#query纠错-之--原理)
      - [Query纠错 之 文本错误类型](#query纠错-之-文本错误类型)
        - [动机](#动机-1)
        - [常见的错误类型](#常见的错误类型)
      - [Query纠错 之 纠错结果类型](#query纠错-之-纠错结果类型)
        - [动机](#动机-2)
        - [介绍](#介绍)
        - [纠错结果类型](#纠错结果类型)
  - [搜索引擎两大问题](#搜索引擎两大问题)
    - [问题一：召回](#问题一召回)
      - [什么是召回？](#什么是召回)
      - [基于关键词的召回方法](#基于关键词的召回方法)
        - [什么是 基于关键词的召回方法 ？](#什么是-基于关键词的召回方法-)
      - [基于关键词的召回方法存在哪些问题？](#基于关键词的召回方法存在哪些问题)
        - [Q1：索引粒度如何选择问题](#q1索引粒度如何选择问题)
        - [Q2：保证 召回 有相关文档数问题](#q2保证-召回-有相关文档数问题)
        - [Q3：召回 候选 query 多样性问题](#q3召回-候选-query-多样性问题)
        - [Q4：召回 候选 query 无语义效果问题](#q4召回-候选-query-无语义效果问题)
      - [基于语义的召回方法](#基于语义的召回方法)
        - [什么是 基于语义的召回方法？](#什么是-基于语义的召回方法)
        - [基于语义的召回方法 的思路](#基于语义的召回方法-的思路)
        - [基于语义的召回方法 存在问题](#基于语义的召回方法-存在问题)
      - [参考资料](#参考资料-1)
    - [问题二：相关性](#问题二相关性)
      - [什么是 相关性？](#什么是-相关性)
      - [相关性 存在哪些问题？](#相关性-存在哪些问题)
      - [相关性方法介绍](#相关性方法介绍)
        - [计算场景角度](#计算场景角度)
        - [计算方法角度](#计算方法角度)
      - [参考资料](#参考资料-2)
  - [搜索未来新趋势](#搜索未来新趋势)
    - [1. 多模态搜索](#1-多模态搜索)
    - [2. 更语义搜索](#2-更语义搜索)
    - [3。 多轮搜索](#3-多轮搜索)

##### [【关于 文本纠错】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_corrector/)

- [【关于 GECToR】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/tree/master/text_corrector/GECToR/)
  - 动机：
    - 由于 NMT-based GEC系统 的 核心是 seq2seq 结构，所以在部署的时候会遇到以下问题：
    1. 缓慢的推理速度；
    2. 需要大量的训练数据；
    3. 可解释性，从而使他们需要其他功能来解释更正，例如语法错误类型分类；
  - 论文方法：提出了仅使用Transformer编码器的简单有效的GEC序列标注器。
  - 论文思路：
    - 系统在综合数据上进行了预训练；
    - 然后分两个阶段进行了微调：
      - 首先是错误的语料库；
      - 其次是有错误和无错误的平行语料库的组合。
    - 我们设计了自定义的字符级别转换，以将输入字符映射到纠正后的目标。
  - 效果：
    - 我们最好的单模型以及联合模型GEC标注器分别在CoNLL-2014测试集上F0.5达到65.3和66.5，在BEA-2019上F0.5达到72.4和73.6。模型的推理速度是基于Transformer的seq2seq GEC系统的10倍


#### 实战篇

##### 重点推荐篇

- [Transfromer 源码实战](https://github.com/km1994/nlp_paper_study/tree/master/transformer_study/Transformer)
  - [【关于 Transformer 代码实战（文本摘要任务篇）】 那些你不知道的事](https://github.com/km1994/nlp_paper_study/blob/master/transformer_study/Transformer/code.md) 【[知乎篇](https://zhuanlan.zhihu.com/p/312044432) 】

- [【关于 Bert 源码解析 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/blob/master/bert_study/T1_bert/)
  - [【关于 Bert 源码解析 之 主体篇 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/blob/master/bert_study/T1_bert/bertCode1_modeling.md)
  - [【关于 Bert 源码解析 之 预训练篇 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/blob/master/bert_study/T1_bert/bertCode2_pretraining.md)
  - [【关于 Bert 源码解析 之 微调篇 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/blob/master/bert_study/T1_bert/bertCode3_fineTune.md)
  - [【关于 Bert 源码解析IV 之 句向量生成篇 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/blob/master/bert_study/T1_bert/bertCode4_word2embedding.md) 
  - [【关于 Bert 源码解析V 之 文本相似度篇 】 那些的你不知道的事](https://github.com/km1994/nlp_paper_study/blob/master/bert_study/T1_bert/bertCode5_similarity.md)

### 会议收集篇

- [ACL2020](other_study/meeting/ACL_study/ACL2020.md)
- [SIGIR2020](other_study/meeting/SIGIR_stduy/readme.md/)
- [【关于 AAAI 】那些你不知道的事](other_study/meeting/AAAI_study/)
  - 一、AAAI 2021
    - 1.1 情感分析
      - 【Learning Modality-Specific Representations with Self-Supervised Multi-Task Learning for Multimodal Sentiment Analysis (Self-MM)】
      - 【An Adaptive Hybrid Framework for Cross-Domain Aspect-Based Sentiment Analysis (AHF)】
      - 【Bridging Towers of Multi-Task Learning with a Gating Mechanism for Aspect-Based Sentiment Analysis and Sequential Metaphor Identification ()】
      - 【Human-Level Interpretable Learning for Aspect-Based Sentiment Analysis ()】
      - 【A Joint Training Dual-MRC Framework for Aspect Based Sentiment Analysis ()】
      - 【Quantum Cognitively Motivated Decision Fusion for Video Sentiment Analysis ()】
      - 【Context-Guided BERT for Targeted Aspect-Based Sentiment Analysis ()】
      - 【Segmentation of Tweets with URLs and its Applications to Sentiment Analysis ()】
      - 【Segmentation of Tweets with URLs and its Applications to Sentiment Analysis ()】
    - 1.2 命名实体识别
      - 【Multi-Modal Graph Fusion for Named Entity Recognition with Targeted Visual Guidance (UMGF)】
      - 【CrossNER: Evaluating Cross-Domain Named Entity Recognition ()】
      - 【A Supervised Multi-Head Self-Attention Network for Nested Named Entity Recognition ()】
      - 【Nested Named Entity Recognition with Partially-Observed TreeCRFs (Partially-Observed-TreeCRFs)】
      - 【Continual Learning for Named Entity Recognition】
      - 【Knowledge-Aware Named Entity Recognition with Alleviating Heterogeneity】
      - 【Denoising Distantly Supervised Named Entity Recognition via a Hypergeometric Probabilistic Model】
      - 【MTAAL: Multi-Task Adversarial Active Learning for Medical Named Entity Recognition and Normalization（MTAAL）】
    - 1.3 关系抽取
      - 【FL-MSRE: A Few-Shot Learning Based Approach to Multimodal Social Relation Extraction（L-MSRE）】
      - 【Multi-View Inference for Relation Extraction with Uncertain Knowledge】
      - 【GDPNet: Refining Latent Multi-View Graph for Relation Extraction（GDPNet）】
      - 【Progressive Multi-Task Learning with Controlled information Flow for Joint Entity and Relation Extraction】
      - 【Curriculum-Meta Learning for Order-Robust Continual Relation Extraction】
      - 【Document-Level Relation Extraction with Reconstruction】
      - 【Document-Level Relation Extraction with Adaptive Thresholding and Localized Context Pooling(ATLOP )】
      - 【Entity Structure Within and Throughout: Modeling Mention Dependencies for Document Level Relation Extraction（SSAN）】
      - 【Empower Distantly Supervised Relation Extraction with Collaborative Adversarial Training(  MULTICAST)】
      - 【Clinical Temporal Relation Extraction with Probabilistic Soft Logic Regularization and Global Inference（CTRL-PG）】
      - 【A Unified Multi-Task Learning Framework for Joint Extraction of Entities and Relations】
    - 1.4 事件抽取
      - 【A Unified Multi-Task Learning Framework for Joint Extraction of Entities and Relations】
      - 【What the Role Is vs. What Plays the Role: Semi-Supervised Event Argument Extraction via Dual Question Answering（DualQA）】
      - 【Span-Based Event Coreference Resolution】
    - 1.5 知识图谱
      - 【Dual Quaternion Knowledge Graph Embeddings(DualE)】
      - 【Type-Augmented Relation Prediction in Knowledge Graphs】
      - 【ChronoR: Rotation Based Temporal Knowledge Graph Embedding】
      - 【PASSLEAF: A Pool-Based Semi-Supervised Learning Framework for Uncertain Knowledge Graph Embedding】
      - 【KG-BART: Knowledge Graph-Augmented Bart for Generative Commonsense Reasoning】
      - 【Answering Complex Queries in Knowledge Graphs with Bidirectional Sequence Encoders】
      - 【其他】

### Elastrsearch 学习篇

- [Elastrsearch 学习](es_study/)
  - [ElasticSearch架构解析与最佳实践.md](es_study/ElasticSearch架构解析与最佳实践.md)
  
### 竞赛篇

#### [【关于 NLP比赛】 那些你不知道的事](nlp_game/) 

- [一、问答匹配任务](#一问答匹配任务)
  - [5. 新冠疫情相似句对判定大赛 【比赛地址】](#5-新冠疫情相似句对判定大赛-比赛地址)
    - [5.1 赛题背景](#51-赛题背景)
    - [5.2 数据集介绍](#52-数据集介绍)
    - [5.3 比赛方案收集](#53-比赛方案收集)
  - [4. 2021搜狐校园文本匹配算法大赛 【比赛地址】](#4-2021搜狐校园文本匹配算法大赛-比赛地址)
    - [4.1 赛题背景](#41-赛题背景)
    - [4.2 比赛任务](#42-比赛任务)
    - [4.3 数据说明 【地址】](#43-数据说明-地址)
    - [4.4 比赛方案收集](#44-比赛方案收集)
  - [3. CCF2020问答匹配比赛](#3-ccf2020问答匹配比赛)
    - [3.1 比赛背景](#31-比赛背景)
    - [3.2 比赛方案收集](#32-比赛方案收集)
  - [2. 智能客服问题相似度算法设计——第三届魔镜杯大赛](#2-智能客服问题相似度算法设计第三届魔镜杯大赛)
  - [1. 2018CIKM AnalytiCup – 阿里小蜜机器人跨语言短文本匹配算法竞赛](#1-2018cikm-analyticup--阿里小蜜机器人跨语言短文本匹配算法竞赛)
  - [其他](#其他)
- [二、对话](#二对话)
  - [1. 2020 CCF BDCI《千言：多技能对话》](#1-2020-ccf-bdci千言多技能对话)
    - [1.1 赛题简介](#11-赛题简介)
    - [1.2 比赛方案收集](#12-比赛方案收集)
  - [2. 2018JD Dialog Challenge 任务导向型对话系统挑战赛](#2-2018jd-dialog-challenge-任务导向型对话系统挑战赛)
- [三、文本分类](#三文本分类)
  - [1. 2018 DC达观-文本智能处理挑战](#1-2018-dc达观-文本智能处理挑战)
  - [2. 路透社新闻数据集“深度”探索性分析(词向量/情感分析)](#2-路透社新闻数据集深度探索性分析词向量情感分析)
  - [3. 知乎看山杯](#3-知乎看山杯)
  - [4. 2018 CCL 客服领域用户意图分类评测](#4-2018-ccl-客服领域用户意图分类评测)
  - [5. 2018 kaggle quora insincere questions classification](#5-2018-kaggle-quora-insincere-questions-classification)
- [四、 关键词提取](#四-关键词提取)
  - [1. “神策杯”2018高校算法大师赛(关键词提取)](#1-神策杯2018高校算法大师赛关键词提取)
- [五、内容识别](#五内容识别)
  - [1. 第二届搜狐内容识别大赛](#1-第二届搜狐内容识别大赛)
- [六、观点主题](#六观点主题)
  - [1. 汽车行业用户观点主题及情感识别](#1-汽车行业用户观点主题及情感识别)
- [七、实体链指](#七实体链指)
  - [7.1. CCKS&2019中文短文本的实体链指](#71-ccks2019中文短文本的实体链指)
  - [7.2. CCKS 2020实体链指比赛](#72-ccks-2020实体链指比赛)
- [八、命名实体识别](#八命名实体识别)
  - [8.1 天池中药说明书实体识别](#81-天池中药说明书实体识别)
    - [8.1.1 任务描述](#811-任务描述)
    - [8.1.2 比赛方案](#812-比赛方案)
  - [8.2 CCF BDCI 中文命名实体识别算法鲁棒性评测](#82-ccf-bdci-中文命名实体识别算法鲁棒性评测)
    - [8.2.1 任务描述](#821-任务描述)
- [九、事件抽取](#九事件抽取)
  - [9.1 CCKS 2020：面向金融领域的小样本跨类迁移事件抽取](#91-ccks-2020面向金融领域的小样本跨类迁移事件抽取)
    - [9.1.1 任务描述](#911-任务描述)
    - [9.1.2 比赛方案](#912-比赛方案)
  - [9.2 CCKS2019_EventEntityExtraction](#92-ccks2019_evententityextraction)
    - [9.1.1 任务描述](#911-任务描述-1)
    - [9.1.2 比赛方案](#912-比赛方案-1)
  - [9.3 2020 科大讯飞事件抽取挑战赛](#93-2020-科大讯飞事件抽取挑战赛)
    - [9.3.1 任务描述](#931-任务描述)
    - [9.3.2 比赛方案](#932-比赛方案)
- [十、阅读理解](#十阅读理解)
  - [10.1 2021海华AI挑战赛·中文阅读理解·技术组](#101-2021海华ai挑战赛中文阅读理解技术组)
    - [10.1.1 赛题背景](#1011-赛题背景)
    - [10.1.2 比赛任务](#1012-比赛任务)
    - [10.1.3 比赛方案](#1013-比赛方案)
- [十一、关系抽取](#十一关系抽取)
  - [11.1 2020语言与智能技术竞赛：关系抽取任务 【比赛链接】](#111-2020语言与智能技术竞赛关系抽取任务-比赛链接)
    - [11.1.1 赛题背景](#1111-赛题背景)
    - [11.1.2 赛题说明](#1112-赛题说明)
    - [11.1.3 数据集介绍](#1113-数据集介绍)
    - [11.1.4 比赛方案](#1114-比赛方案)
- [十二、中文文本纠错](#十二中文文本纠错)
  - [12.1 专业赛：自然语言处理技术创新大赛——中文文本纠错比赛](#121-专业赛自然语言处理技术创新大赛中文文本纠错比赛)
    - [12.1.1 竞赛背景](#1211-竞赛背景)
    - [12.1.2 赛题描述](#1212-赛题描述)
    - [12.1.3 模型训练](#1213-模型训练)
    - [12.1.4 训练集数据介绍](#1214-训练集数据介绍)
    - [12.1.5 比赛方案](#1215-比赛方案)
- [十三、智能人机交互自然语言理解](#十三智能人机交互自然语言理解)
  - [13.1 CCF BDCI 智能人机交互自然语言理解](#131-ccf-bdci-智能人机交互自然语言理解)
    - [13.1.1 竞赛背景](#1311-竞赛背景)
    - [13.1.2 数据集介绍](#1312-数据集介绍)
- [十四、智能人机交互自然语言理解](#十四智能人机交互自然语言理解)
  - [14.1 CCF BDCI 预训练模型知识量度量](#141-ccf-bdci-预训练模型知识量度量)
    - [14.1.1 竞赛背景](#1411-竞赛背景)
    - [14.1.2 数据集介绍](#1412-数据集介绍)
- [参考资料](#参考资料)

#### [【关于 NLP 比赛方案学习】 那些你不知道的事](nlp_game/game_study/)

##### [【关于 NLP 比赛方案学习】 那些你不知道的事](nlp_game/game_study/)

- [实体链指](nlp_game/game_study/实体链指/)
  - [CCKS&2019中文短文本的实体链指](nlp_game/game_study/实体链指/CCKS&2019中文短文本的实体链指)
    - [CCKS2019中文短文本实体链指比赛技术创新奖解决方案](nlp_game/实体链指/CCKS&2019中文短文本的实体链指/CCKS2019中文短文本实体链指比赛技术创新奖解决方案)
    - [CCKS2020实体链指比赛小米KG冠军方案](nlp_game/实体链指/CCKS&2019中文短文本的实体链指/CCKS2020实体链指比赛小米KG冠军方案)


### [学习资源]()

- [知识图谱]()
  - [东南大学《知识图谱》研究生课程](https://github.com/npubird/KnowledgeGraphCourse)
  - [基于知识图谱的金融资讯推荐](https://github.com/codeants2012/FinancialKnowledgeGraph)
  - [北京知识图谱学习小组](https://github.com/memect/kg-beijing)
  - 美团技术团队文章
    - [领域应用 | 常识性概念图谱建设以及在美团场景中的应用](https://mp.weixin.qq.com/s/FFkcu5K1oZnzX8Rg72WHqQ)
    - [【实践】多业务建模在美团搜索排序中的实践](https://mp.weixin.qq.com/s/itAj4jvL1lR4CfbL2rkl_w)
    - [美团外卖美食知识图谱的迭代及应用](https://mp.weixin.qq.com/s/JX9xUgxcniNLlmKDR7AAGA)
- [文本摘要]()
  - [Summarization.](https://github.com/bifeng/nlp_paper_notes/blob/75cf64a7eb244814fccf241d5990e23526352ab3/Summarization.md)
  - [GPT2-NewsTitle](https://github.com/liucongg/GPT2-NewsTitle)
- [CLUEDatasetSearch](https://github.com/CLUEbenchmark/CLUEDatasetSearch)【中英文NLP数据集】

### [NLP 数据集](nlp_corpus/)

- [【关于 NLP 语料】那些你不知道的事](nlp_corpus/)
  - 一、命名实体识别
    1. [boson数据集](nlp_corpus/ner_data/boson/)
    2. [clue细粒度实体识别数据集](nlp_corpus/ner_data/cluener_public/)
    3. [微软实体识别数据集](nlp_corpus/ner_data/MSRA/)
    4. [人民网实体识别数据集（98年）](nlp_corpus/ner_data/people_daily/)
    5. [中药说明书实体识别数据集（“万创杯”中医药天池大数据竞赛）](nlp_corpus/ner_data/tianchi_yiyao/)
    6. [视频_音乐_图书数据集](nlp_corpus/ner_data/video_music_book_datasets/)
    7. [微博数据集](nnlp_corpus/er_data/weibo/)
    8. [简历 数据集](nlp_corpus/ner_data/ResumeNER/)
    9. [2020_ccks_ner 中文医学文本命名实体识别](nlp_corpus/ner_data/2020_ccks_ner/)
  - [二、抽取式文本摘要](nlp_corpus/chinese_abstractive_corpus)
    1. [教育培训行业抽象式自动摘要中文语料库](nlp_corpus/chinese_abstractive_corpus/education/)【中文】
    2. [哈工大-新浪微博短文本摘要](https://pan.baidu.com/share/init?surl=szq0Wa60AS5ISpM_SNPcbA)【密码：ayn6】【中文】
    3. [教育培训行业抽象式自动摘要中文语料库](nlp_corpus/chinese_abstractive_corpus/education/)【中文】
    4. [个人-新浪微博](https://pan.baidu.com/s/1NWe6K33GMTp4Wk7CwaGotA)【密码：4k12】【中文】
    5. [港大多文本摘要](nlp_corpus/chinese_abstractive_corpus/港大多文本摘要/) 【英文】
    6. [WikiHow: A Large Scale Text Summarization Dataset](https://github.com/mahnazkoupaee/WikiHow-Dataset) 【英文】
    7. [The CNN / Daily Mail dataset (non-anonymized)](https://github.com/abisee/cnn-dailymail) 【英文】
    8. [Scientific Document Summarization Corpus and Annotations from the WING NUS group](https://github.com/WING-NUS/scisumm-corpus) 【英文】【Data and code for the AAAI 2019 paper cisummNet: A Large Annotated Corpus and Content-Impact Models for Scientific Paper Summarization with Citation Networks】
    9. [Multi-News](https://github.com/Alex-Fabbri/Multi-News) 【英文】【介绍：Data and code for the ACL 2019 paper Multi-News: a Large-Scale Multi-Document Summarization Dataset and Abstractive Hierarchical Model.】

### [GCN_study学习篇](https://github.com/km1994/GCN_study)

- GCN 介绍篇
  - [Graph 介绍](https://github.com/km1994/GCN_study/blob/master/graph_introduction/graph_introduction.md)
  - [Weisfeiler-Leman 算法介绍](https://github.com/km1994/GCN_study/blob/master/WL/WL_conclusion.md)

- GCN 三剑客
  - [Convolutional Neural Networks on Graphs with Fast Localized Spectral Filtering](https://github.com/km1994/GCN_study/blob/master/CNNonGraph_Defferrard_2016/CNNonGraph_Defferrard_2016_总结.md)
  - [SEMI-SUPERVISED CLASSIFICATION WITH GRAPH CONVOLUTIONAL NETWORKS](https://github.com/km1994/GCN_study/blob/master/GCN/SEMI-SUPERVISED%20CLASSIFICATION%20WITH%20GRAPH%20CONVOLUTIONAL%20NETWORKS.pdf)
  - [Attention Models in Graphs: A Survey](https://github.com/km1994/GCN_study/blob/master/Attention_models/Attention_models.md)

- 经典篇
  - [Can GNN go “online”?an analysis of pretraining and inference](https://github.com/km1994/GCN_study/tree/master/CanGNNGoOnline)
  - [Graph Convolutional Networks for Text Classification](https://github.com/km1994/GCN_study/tree/master/GCNforTextClassification)
  - [HOW POWERFUL ARE GRAPH NEURAL NETWORKS](https://github.com/km1994/GCN_study/blob/master/HowPowerGCN/HOW%20POWERFUL%20ARE%20GRAPH%20NEURAL%20NETWORKS.pdf)
  - [Graph Convolutional Matrix Completion](https://github.com/km1994/GCN_study/blob/master/GCMC/Graph%20Convolutional%20Matrix%20Completion.pdf)
  - [Representation Learning For Attributed Multiplex Heterogeneous Network](https://github.com/km1994/GCN_study/blob/master/RepresentationLearningForAttributedMultiplexHeterogeneousNetwork/RepresentationLearningForAttributedMultiplexHeterogeneousNetwork.md)

- 预训练篇
  - [GNN 教程：GCN 的无监督预训练](https://github.com/km1994/GCN_study/tree/master/pretrainingGCN_1)
  - [Pre-training Graph Neural Networks](https://github.com/km1994/GCN_study/blob/master/pretrainingGCN_2/pretrainingGCN.md)

- 实战篇
  - [DGL](https://github.com/km1994/dgl)
  - [DGL 入门](https://github.com/km1994/GCN_study/blob/master/DGL_study/DGL_introduction.md)
  - [DGL 入门 —— GCN 实现](https://github.com/km1994/GCN_study/blob/master/DGL_study/DGL_GCN_introduction.md)

## 参考资料

1. [【ACL2020放榜!】事件抽取、关系抽取、NER、Few-Shot 相关论文整理](https://www.pianshen.com/article/14251297031/)
2. [第58届国际计算语言学协会会议（ACL 2020）有哪些值得关注的论文？](https://www.zhihu.com/question/385259014)

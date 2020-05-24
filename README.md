# NLP-Paper 前沿追踪

# Commonsense Reasoning models
1. **[AAAI2020]** Joint Commonsense and Relation Reasoning for Image and Video Captioning（联合常识和关系推理用于图像和视频描述）
> 简介：本文的方法是通过常识推理和关系推理的迭代学习算法交替实现的，常识推理将视觉区域嵌入语义空间以构建语义图，关系推理用于编码语义图以生成句子。C-R Reasoning 方法包括三个模块，如图 1.2 所示。视觉映射和知识映射模块（Visual Mapping & knowledge mapping）在生成语义实体候选后，通过视觉映射学习语义实体候选的视觉特征向量，通过知识映射来学习候选的知识向量。常识推理模块(Common sense)根据给定的候选，在先验知识图的指导下构建语义图。关系推理模块 (Relation Reasoning)中根据给定的语义图，通过图卷积网络 (GCN) 和基于序列的语言模型来生成文本描述。

2. **[AAAI2020]** Graph-Based Reasoning over Heterogeneous External Knowledge for Commonsense Question Answering（利用异构外部知识基于图的推理进行常识知识问答）

> 简介：来自结构化的知识源（如 ConceptNet）包含概念之间的宝贵结构关系，对于推理很有帮助，但是它们的覆盖率低。而纯文本知识源（如维基百科）是对结构化知识的补充，可以提供丰富且覆盖面广的证据。最近的研究还没有同时利用这两类知识源进行推理的，因此在这项工作中，作者提议自动从这两个异构知识源中提取证据，并根据提取的证据回答问题。

3. **[AAAI2020]** Commonsense Knowledge Base Completion with Structural and Semantic Context（利用结构和语义上下文的常识知识库实现）

4. **[AAAI2020]** Understanding the semantic content of sparse word embeddings using a commonsense knowledge base（使用常识知识库理解稀疏词嵌入的语义内容）

5. **[AAAI2020]** Evaluating Commonsense in Pre-trained Language Models（在预训练语言模型中评估常识）

6. **[AAAI2020]** KnowIT VQA: Answering Knowledge-Based Questions about Videos（KnowIT VQA：回答关于视频的知识问题）

7. **[ICLR2020]** Abductive Commonsense Reasoning(常识性的溯因推理)

> 简介：首先提出溯因推理在文本上的研究，提出了ART数据集，包括NLI和NLG两个任务

8. **[ACL2019]** Explain Yourself! Leveraging Language Models for Commonsense Reasoning.

> 简介：主要亮点是利用预训练语言模型中的丰富信息生成解释，辅助CQA(Commonsense Question Answer)任务，对比CQA的the state of the art baseline，提升了10%的准确率。文章中的CQA任务被分解为两步，（1）Commonsense Auto-Generated Explanations (CAGE)：Explanation的生成利用conditional language model完成，根据输入条件的不同分为reasoning与rationalization两种。（2）Commonsense Predictions with Explanations：使用Bert模型进行分类，CQA的原始输入中再加入生成的或者人为标注的explanation。

9. **[EMNLP2019]** KagNet: Knowledge-Aware Graph Networks for Commonsense Reasoning

> 简介：提出了一个Knowledge-aware reasoning 框架，主要有两个步骤:（1）schema graph grounding（2）graph modeling for inference

10. **[ACL2018]** Extracting Commonsense Properties from Embeddings with Limited Human Guidance(从词嵌入中提取常识属性)

> 简介：这是ACL2018的short paper，主要是在acl2017提出的VERB PHYSICS数据集上做的，这个数据集只有5个属性，数据集的原文使用概率因子图做的，这篇论文就很简单得使用词嵌入空间映射的方法做的，而且提出了升级版的数据集PROPERTY COMMON SENSE data


# Commonsense Reasoning datasets

1. **[AAAI2020]** PIQA: Reasoning about Physical Commonsense in Natural Language(物理交互问答:自然语言中的物理常识推理)

> 简介：「在不使用刷子涂眼影的情况下，我应该用棉签还是牙签？」类似这种需要物理世界常识的问题对现今的自然语言理解系统提出了挑战。虽然最近的预训练模型 (如 BERT) 在更抽象的如新闻文章和百科词条这种具有丰富文本信息的领域问答方面取得了进展，但在更现实的领域，由于报导的偏差，文本本质上是有限的，类似于「用牙签涂眼影是一个坏主意」这样的事实很少得到直接报道。人工智能系统能够在不经历物理世界的情况下可靠地回答物理常识问题吗？是否能够捕获有关日常物品的常识知识，包括它们的物理特性、承受能力以及如何操纵它们。在本文中，作者介绍了一个关于物理常识推理任务和相应的基准数据集 PIQA（Physical Interaction：Question Answering）进行评估。虽然人类应对这一数据集很容易 (95% 的准确率)，但是大型的预训模型很难 (77%)。作者分析了现有模型所缺乏的知识为未来的研究提供了重要的机遇。

参考： <br/>
[1] https://zhuanlan.zhihu.com/nlu-mrc-ongoing <br/>
[2] https://zhuanlan.zhihu.com/p/109886447

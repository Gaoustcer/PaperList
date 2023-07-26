# Paper List

## Domain Adaptation

### Traditional Representation Method

| 工作       | 链接                                                      | 主要内容                                                     |
| ---------- | --------------------------------------------------------- | ------------------------------------------------------------ |
| LUSR       | [Arxiv](https://arxiv.org/abs/2102.05714)                 | 借助Disentanglement VAE将state分解为Specific/Unspecific两部分，后者用于迁移 |
| CURL       |                                                           | 对比学习方法构建正负样本对，获得正样本对之间的不变表示，学习cross-Domain的不变特征 |
| CARLA      |                                                           | 预训练降噪自编码器(DAE)学习对输入鲁棒的表征，将状态之间的距离转化为降噪自编码器编码空间上的距离 |
| DBC        |                                                           | 从环境的动态信息(状态转移/奖励函数)角度刻画状态之间的距离，译码器输出的状态距离应该正比于状态在环境中的动态距离 |
| RecycleGAN |                                                           | 构建Sim2Real和Real2Sim两个GAN，假设GAN满足Cycle Consistency，得到Sim2Sim和Real2Real的等价变换，要求value function对于转换后的状态具有不变性 |
| DARC       |                                                           | 通过Target/Source Domain上状态转移的差异在Source Environment的奖励函数上增添一个启发式函数，用于修正Target/Source Domain之间的差异 |
| TED        | [Arxiv](https://arxiv.org/pdf/2207.05480.pdf)             | 对抗学习+对比学习，将时序上连续的state作为正样本，同时训练一个Classifier用于区分时序上连续/离散的样本以训练Encoder |
| DrQ        | [Openreview](https://openreview.net/forum?id=GY6-6sTvGaf) | CURL去掉对比学习模块，使用数据增强提高强化学习泛化性，要求value function对于不同Data Augmentation保持不变 |

### Vision Language Model(VLM) and Prompt Learning

| 工作   | 链接 | 主要内容                                                     |
| ------ | ---- | ------------------------------------------------------------ |
| CLIP   |      | 针对分类模型不能泛化到没有见过的分类这一问题，作者提出了一种新的基于弱监督信号的预训练视觉语言模型的新方法，预训练数据采取用title的图片数据，这些数据从互联网上收集得到而不需要人为标注。对于下游任务(分类)采取设计合适的prompt，根据prompt和image encode的结果相似度进行分类。实验证明在一些数据集上做zero-shot transfer的效果和监督模型类似 |
| CoOp   |      | 讨论如何通过模型学到一个好的Prompt，解决了CLIP中特定数据集的Prompt需要依赖专家知识手动生成的难点 |
| CoCoOp |      | 针对CoOp学到的Unified Context Representation无法泛化到同一个task unseen class的问题，在Context Learning分支增添一支使得Context Embedding和Image Embedding相关 |



### Domain Adaptation via Prompt Tuning and Vision Language Model(VLM)

| 工作 | 链接 | 主要内容 |
| ---- | ---- | -------- |
|      |      |          |
|      |      |          |
|      |      |          |


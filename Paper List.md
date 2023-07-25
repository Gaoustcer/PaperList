# Paper List

## Domain Adaptation

### Traditional Representation Method

| 工作       | 链接                                      | 主要内容                                                     |
| ---------- | ----------------------------------------- | ------------------------------------------------------------ |
| LUSR       | [Arxiv](https://arxiv.org/abs/2102.05714) | 借助Disentanglement VAE将state分解为Specific/Unspecific两部分，后者用于迁移 |
| CURL       |                                           | 对比学习方法构建正负样本对，获得正样本对之间的不变表示，学习cross-Domain的不变特征 |
| CARLA      |                                           | 预训练降噪自编码器(DAE)学习对输入鲁棒的表征，将状态之间的距离转化为降噪自编码器编码空间上的距离 |
| DBC        |                                           | 从环境的动态信息(状态转移/奖励函数)角度刻画状态之间的距离，译码器输出的状态距离应该正比于状态在环境中的动态距离 |
| RecycleGAN |                                           | 构建Sim2Real和Real2Sim两个GAN，假设GAN满足Cycle Consistency，得到Sim2Sim和Real2Real的等价变换，要求value function对于转换后的状态具有不变性 |
| DARC       |                                           | 通过Target/Source Domain上状态转移的差异在Source Environment的奖励函数上增添一个启发式函数，用于修正Target/Source Domain之间的差异 |
| TED        |                                           | 对抗学习+对比学习，将时序上连续的state作为正样本，同时训练一个Classifier用于区分时序上连续/离散的样本以训练Encoder |
| DrQ        |                                           | CURL去掉对比学习模块，使用数据增强提高强化学习泛化性，要求value function对于不同Data Augmentation保持不变 |



### Domain Adaptation via Prompt Tuning and Vision Language Model(VLM)

| 工作 | 链接 | 主要内容 |
| ---- | ---- | -------- |
|      |      |          |
|      |      |          |
|      |      |          |


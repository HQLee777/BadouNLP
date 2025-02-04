## 郑昕第二周作业

### 目标：
- 训练多类分类模型，根据预定义规则预测5维输入向量的类别。该模型的输出是跨多个类别的概率分布。
- 通过最小化交叉熵损失来训练模型，使其正确地对输入向量进行分类，交叉熵损失将预测的概率分布与真实的类别标签进行比较。

### 任务规则：

1. 输入数据：每个输入都是一个向量 x = [x_1, x_2, x_3, x_4, x_5] ，其中每个 x_i 是 0 到 1 之间的随机数。
2. 分类规则：根据哪个特定子集的分量之和最大，将向量分配到三个类 \{0, 1, 2\} 中的一个： 
- 类 0：如果 \text{前两个分量之和 } (x_1 + x_2) 最大。
- 类 1：如果 \text{中间两个分量之和 } (x_3 + x_4) 最大。
- 类 2：如果 \text{最后一个分量和第一个分量之和 } (x_5 + x_1) 最大。0
3. 输出：
- 模型输出三个类别 \{0, 1, 2\} 的概率分布。
- 例如：\text{Output} = [0.7, 0.2, 0.1] 表示模型预测 0 类的置信度为 70%，1 类的置信度为 20%，2 类的置信度为 10%。
4. 评估：
- 根据准确度以及预测概率与真实标签的匹配程度来评估模型的性能。



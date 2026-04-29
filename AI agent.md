# LLM
large language model
基于transformer架构 (attention is all you need)
## 1 工作原理
文字接龙游戏，预测下一个词，追加回输入信息继续预测。
## 2 Token
大模型处理文本的**最基本
大模型是一个函数，里面跑的是矩阵运算，接受的是**数字**，输出的也是数字。
人类和大模型之间的Tokenizer：负责编码和解码。
编码的具体过程：Tokenizer切分文字，对每个Token进行映射，变成一串Token ID组成的列表

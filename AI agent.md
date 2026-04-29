# LLM
large language model
基于transformer架构 (attention is all you need)
## 1 工作原理
文字接龙游戏，预测下一个词，追加回输入信息继续预测。
## 2 Token
大模型处理文本的**最基本单元**
大模型是一个函数，里面跑的是矩阵运算，接受的是**数字**，输出的也是数字。
人类和大模型之间的Tokenizer：负责编码和解码。
编码的具体过程：Tokenizer切分文字，对每个Token进行映射，变成一串Token ID组成的列表
Token和词并没有一一对应关系  ==为什么没有，或者说为什么要有==
平均来说1个Token对应0.75个单词，1.5-2个汉字。==一般来说为了表达同样的意思，所需要的英文单词数是中文字数的1.5倍。所以，大模型在处理中文命令时是不是耗费的Token数会更少，而传达出的信息量相当。这条逻辑链有问题吗？==
使用BPE算法训练和使用Tokenizer
## 3 Context
大模型每次处理任务时所收到的**信息总和**
大模型本质上不具有记忆功能
程序会将用户问题和对话历史一起发送给大模型
### Context Window
上下文窗口，Context所能容纳的最大Token数量
目前主流模型的Context Window大小在100万左右 (GPT5.4, Gemini 3.1pro, Claude Opus 4.6)
## 4 Prompt
大模型接收的具体问题或指令

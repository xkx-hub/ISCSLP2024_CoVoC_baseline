# ISCSLP2024_CoVoC_baseline

本次竞赛baseline共有两个模型

## 模型一：VALL-E 
基于开源代码Amphion训练，训练过程分为两步，首先在Wenetspeech4TTS数据集上进行训练，之后在HQ-Conversations进行微调训练。

模型的权重部分已经在huggface开源

训练过程中，文本输入的方式与原Amphion代码略有不同，具体方式见inference.ipynb

文本转音素代码参考BertVits2


## 模型二
基于fish-speech的开源模型训练，微调了其中的LLAMA 与 vits_decoder

模型权重部分已经在huggface开源

训练遵循fish-speech的默认配置

具体训练代码请参考fish-speech


## 鸣谢
- [Bert-VITS2](https://github.com/fishaudio/Bert-VITS2)
- [Amphion](https://github.com/open-mmlab/Amphion)
- [Fish-Speech](https://github.com/fishaudio/fish-speech)

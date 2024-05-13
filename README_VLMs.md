# awesome-list-of-LLM_VLMs🌐✨
github awesome list of recent LLMs and VLMs.

Here is list of **VLMs**, to reach list of LLMs. Click [here](https://github.com/HuBocheng/awesome-list-of-LLM_VLMs/blob/master/README.md)🚀



## Quick Start🏁

|   Model    |       Parameters        |                             Demo                             |                          CheckPoint                          | Details |
| :--------: | :---------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :-----: |
| MiniGemini |       7B/13B/70B        |                                                              | [Llama2 Family](https://huggingface.co/collections/meta-llama/llama-2-family-661da1f90a9d678b6f55773b) |    [MiniGemini](#minigemini)     |
|   Bunny    |         8B/70B          |                                                              | [Llama3 Family](https://huggingface.co/collections/meta-llama/meta-llama-3-66214712577ca38149ebb2b6) |     [Bunny](#bunny)    |
|   Llava    | 0.5B/1.8B/4B/7B/14B/72B |                                                              |             [Qwen](https://huggingface.co/Qwen)              |    [Llava](#llava)     |
| Cog Series | 0.5B/1.8B/4B/7B/14B/72B | [CogVLM & CogAgent](https://huggingface.co/spaces/THUDM/CogVLM-CogAgent) |            [Qwen1.5](https://huggingface.co/Qwen)            |    [Cog Series](#cog-series)      |
|    HPT     |       7B/13B/33B        |                                                              |            [Vicuna](https://huggingface.co/lmsys)            |    [HPT](#hpt)    |



## Details Regarding Models Above

### MiniGemini


<a href='https://arxiv.org/pdf/2403.18814.pdf'><img src='https://img.shields.io/badge/Paper-Arxiv-red'></a>
<a href='https://huggingface.co/collections/YanweiLi/mgm-6603c50b9b43d044171d0854'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Models-blue'></a>
<a href='https://huggingface.co/collections/YanweiLi/mgm-data-660463ea895a01d8f367624e'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Data-green'></a>

### Bunny





### Llava



### Cog Series

#### CogVLM

[![arXiv](https://img.shields.io/badge/arXiv-2311.03079-b31b1b.svg)](https://arxiv.org/abs/2311.03079) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/THUDM/CogVLM)

CogVLM is an innovative open-source visual language model (VLM) designed to bridge the gap between traditional language models and visual data processing. It introduces a "visual expert module" within its architecture to enhance the integration of visual and language features without increasing computational demands. This module is embedded in both the attention and feedforward neural network (FFN) layers of a pre-trained language model, allowing for a deep fusion of visual and linguistic data.

Unlike previous methods that often used a shallow alignment strategy, CogVLM achieves a more profound integration by allowing direct interactions between visual and textual representations within the model's layers. This approach enables the model to maintain high performance on natural language processing tasks while also excelling in tasks that require understanding of visual content

  |          模型名称           | 输入分辨率 |                             介绍                             |                      Huggingface model                       |                       SAT model                       |
  | :-------------------------: | :--------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :---------------------------------------------------: |
  |      cogvlm-chat-v1.1       |    490     |      支持同时进行多轮聊天和视觉问答，支持自由的提示词。      |     [link](https://huggingface.co/THUDM/cogvlm-chat-hf)      | [link](https://huggingface.co/THUDM/CogVLM/tree/main) |
  |       cogvlm-base-224       |    224     |               文本-图像预训练后的原始检查点。                |   [link](https://huggingface.co/THUDM/cogvlm-base-224-hf)    | [link](https://huggingface.co/THUDM/CogVLM/tree/main) |
  |       cogvlm-base-490       |    490     | 通过从 cogvlm-base-224 进行位置编码插值，将分辨率提升到490。 |   [link](https://huggingface.co/THUDM/cogvlm-base-490-hf)    | [link](https://huggingface.co/THUDM/CogVLM/tree/main) |
  | cogvlm-grounding-generalist |    490     |    此检查点支持不同的视觉定位任务，例如REC，定位字幕等。     | [link](https://huggingface.co/THUDM/cogvlm-grounding-generalist-hf) | [link](https://huggingface.co/THUDM/CogVLM/tree/main) |



##### 动机

CogVLM的作者认为浅层对齐方法之所以性能较差，是因为它们依赖于“冻结”的语言模型权重，这些权重经过内在训练以处理文本标记，存在严重的不匹配。



##### 创新点

1. 为了防止直接在新数据集上训练LLM导致的遗忘问题和对原数据集的不熟悉，想要在保证原有NLP性能的前提下增加设觉理解能力
2. CogVLM在语言模型中增加了一个可训练的视觉专家（visual expert）。在处理视觉和语言信息时，视觉信息会通过一个专门的机制来处理，而不是简单地将图像特征融入原有的文本处理流程。
   - 在每一层中，图像特征使用新的QKV（Query-Key-Value）矩阵和MLP（多层感知机）层，独立于文本特征进行处理。
3. 使用RoPE（Rotary Positional Embedding），而不是传统位置编码（在传统的Transformer模型中，位置编码通常是与输入序列的词嵌入相加的方式来提供序列中每个元素的位置信息。）

CogVLM在语言模型中增加了一个可训练的视觉专家（visual expert）。这意味着在处理视觉和语言信息时，视觉信息会通过一个专门的机制来处理，而不是简单地将图像特征融入原有的文本处理流程。



##### Architecture

<div align="center">
  <img src="./image/cogVLM.png" alt="image-20240510165317066" width="600" />
</div>




##### 细分

- **CogVLM-Chat**: 模型接受自然语言输入和输出，主要处理纯文本输入和输出，适用于多种VQA和多轮对话数据集
- **CogVLM-Grounding**：侧重于处理包含边界框的输入和输出，支持视觉基准相关的多种任务



##### some tips

LLM是在Vicuna-7B的基础上训练得来的，保证其NLP能力的前提下加上了视觉理解

用到了P-Tuning和LoRA两种高效微调方法



#### CogAgent

[![arXiv](https://img.shields.io/badge/arXiv-2312.08914-b31b1b.svg)](https://arxiv.org/abs/2312.08914) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/THUDM/CogVLM)

**CogAgent** 是一个基于CogVLM改进的开源视觉语言模型，在CogVLM的基础上主要侧重提升了GUI理解和导航能力，能够识别微小的页面元素和文本，在处理屏幕截图相关的任务上优于基于 LLM 的方法。

> 可以好好看一下github和论文中的示例，可以对Agent的概念有一个直观感受和了解。


  |   模型名称    | 输入分辨率 |                             介绍                             |                   Huggingface model                   |                        SAT model                        |
  | :-----------: | :--------: | :----------------------------------------------------------: | :---------------------------------------------------: | :-----------------------------------------------------: |
  | cogagent-chat |    1120    |    CogAgent的聊天版本。支持GUI代理，多轮聊天和视觉定位。     | [link](https://huggingface.co/THUDM/cogagent-chat-hf) | [link](https://huggingface.co/THUDM/CogAgent/tree/main) |
  | cogagent-vqa  |    1120    | CogAgent的VQA版本。在单轮视觉对话中具有更强的能力。推荐用于VQA基准测试。 | [link](https://huggingface.co/THUDM/cogagent-vqa-hf)  | [link](https://huggingface.co/THUDM/CogAgent/tree/main) |

##### 动机

- 完成一个智能体的构建，改智能体在面向GUI的领域中有着非常好的性能。



##### 创新点

- **可以处理高分辨率图像**：该工作设计了一个交叉注意力分支，允许在适当的计算预算内在分辨率和隐藏大小之间进行权衡，缓解高分辨率图像需要大量资源推理和计算的问题。
  - **高分辨率交叉模块**充当更高分辨率输入的新分支，采用了更小的预训练视觉编码器，并使用小隐藏尺寸的交叉注意力将高分辨率图像特征与VLLM解码器的每一层融合在一起，从而降低计算成本。
  - **与低分辨率输入分支的对比**：不同于原始的低分辨率输入分支，高分辨率交叉模块采用了一个更小的预训练视觉编码器（在这里是 EVA2-CLIP-L 的视觉编码器，有 0.30B 参数）。这个模块使用较小的隐藏层尺寸的交叉注意力（cross-attention）来融合高分辨率图像特征与视觉语言长期记忆模型（VLLM）解码器的每一层。
  - 对于一个输入图像，模型会将其重新调整尺寸到 1120 × 1120 和 224 × 224，分别送入高分辨率交叉模块和低分辨率分支。这两个分支并行工作，将图像编码为特征序列 Xhi（高分辨率图像特征）和 Xlo（低分辨率图像特征）
- 私人构建的数据集：They notice that the GUI images share a different distribution from natural images. They thus construct a large-scale annotated dataset about GUIs and OCR for continual pre-training.

##### Architecture

<div align="center">
  <img src="./image/cogAgent.png" alt="image-20240510171107123" width="600" />
</div>



### HPT
[![AI Blog](https://img.shields.io/badge/AI%20Blog-hypergai%20AI-orange.svg)](https://hypergai.com/blog/) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/HyperGAI/HPT/) 

提出的Hyper-Pretrained Transformers（HPT）框架，是一种全新的多模态LLM预训练框架。它能够以高效和可扩展的方式训练出一个大型的多模态基础模型，这个模型能够理解多种模态的输入。有HPT Pro与HPT Air两个版本。

##### 创新点

- 创新特性H-Former作为视觉与语言模态之间的桥梁，是Q-Former的变种
- H-Former 集成了双网络设计，以学习局部和全局特征，以实现视觉语言对齐，使 HPT 能够理解细粒度细节和抽象的高级信息

##### Architecture

<div align="center">
  <img src="./image/HPT.png"  width="600" />
</div>





最新的VLMs survey存储库，包括VLM预训练、迁移学习方法和知识蒸馏方法，还有可以使用的数据集汇总：[github](https://github.com/jingyi0000/VLM_survey)

## 模型评估汇总

Hugging face中的实时排行榜：[Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)


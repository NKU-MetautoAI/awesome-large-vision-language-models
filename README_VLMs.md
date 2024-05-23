# awesome-list-of-LLM_VLMs🌐✨
github awesome list of recent LLMs and VLMs.

Here is list of **VLMs**, to reach list of LLMs. Click [here](https://github.com/HuBocheng/awesome-list-of-LLM_VLMs/blob/master/README.md)🚀



## Quick Start🏁

按发布时间排序

|   Model    |       Parameters        |                             Demo                             |                          CheckPoint                          | Details |
| :--------: | :---------------------: | :----------------------------------------------------------: | :----------------------------------------------------------: | :-----: |
| MiniGemini<br />(MGM) |       2B/7B/13B/34B       | [MGM](https://huggingface.co/spaces/jiaqianjing/Mini-Gemini) | [MGM  Family](https://huggingface.co/collections/YanweiLi/mgm-6603c50b9b43d044171d0854) |    [MiniGemini](#minigemini)     |
|   Bunny    |         2B/3B/4B/8B         | [Bunny](http://bunny.dataoptim.org/) | [BAAI](https://huggingface.co/BAAI) |     [Bunny](#bunny)    |
|   Llava    | 7B/13B | [Llava v1.6](https://huggingface.co/spaces/liuhaotian/LLaVA-1.6) | [Llava v1.5](https://huggingface.co/collections/liuhaotian/llava-16-65b9e40155f60fd046a5ccf2)<br />[Lava v1.6](https://huggingface.co/collections/liuhaotian/llava-15-653aac15d994e992e2677a7e) |    [Llava](#llava)     |
| Cog Series |    17B/18B    | [CogVLM & CogAgent](https://huggingface.co/spaces/THUDM/CogVLM-CogAgent) |            [THUDM ](https://huggingface.co/THUDM)            |    [Cog Series](#cog-series)      |
|    HPT     |       3-8B/6B | None |            [HPT](https://huggingface.co/HyperGAI)            |    [HPT](#hpt)    |
| MiniGPT4 Series | 7B/13B | Invalid Now | [Vision-CAIR ](https://huggingface.co/Vision-CAIR) | [MiniGPT4 Series](#minigpt4-series) |
| TinyLLaVA | 1.4B/2.4B/3.1B | None | [TinyLLaVA](https://huggingface.co/tinyllava) | [TinyLLaVA](#tinyllava) |
| TinyGPT-V | --- | [TinyGPT-V](https://huggingface.co/spaces/llizhx/TinyGPT-V) | [TinyGPT-V](https://huggingface.co/Tyrannosaurus/TinyGPT-V) | [TinyGPT-V](#tinygptv) |
| PaliGemma | 3B | [PaliGemma](https://huggingface.co/spaces/big-vision/paligemma) | [PaliGemma Family](https://huggingface.co/collections/google/paligemma-ft-models-6643b03efb769dad650d2dda) | [PaliGemma](#paligemma) |
| PaLI-3 | 5B | None | None(PaliGemma is based on PaLI-3) | [PaLI-3](#palI3) |
| MobileVLM Series | 1.4B/1.7B/2.7B/7B | Invalid Now | [mtgv](https://huggingface.co/mtgv) | [MobileVLM](#mobilevlm) |
| LLaVA-Phi | 3B | None | None | [LLaVA-Phi](#llavaphi) |
| LLaVA-Phi-3-mini | --- | None | [LLaVA-Phi-3-mini](https://huggingface.co/collections/xtuner/llava-phi-3-mini-662a5f7b9416630a1ad91102) | [LLaVA-Phi-3-mini](#llavaphi3mini) |
| IMP | 3B | [xmbot.net](https://xmbot.net/imp/) | [imp-v1-3b ](https://huggingface.co/MILVLG/imp-v1-3b) | [IMP](#imp) |
| MoE-LLaVA | 3B | [MoE LLaVA](https://huggingface.co/spaces/LanguageBind/MoE-LLaVA) | [MoE-LLaVA Family](https://huggingface.co/collections/LanguageBind/moe-llava-model-65b607bf2524ac36e733874c) | [MoE-LLaVA](#moe-llava) |
| Cobra | 3.5B | [Cobra]([Cobra - a Hugging Face Space by han1997](https://huggingface.co/spaces/han1997/cobra)) | [Cobra Family]([Cobra - a han1997 Collection (huggingface.co)](https://huggingface.co/collections/han1997/cobra-6615c3242851ba108027105d)) | [Cobra](#cobra) |
| Vary-toy |  |  |  |  |
| SPHINX-Tiny |  |  |  |  |
| ALLaVA-Longer |  |  |  |  |
| MM1 |  |  |  |  |
| MiniCPM-V |  |  |  |  |
| DeepSeek-VL |  |  |  |  |
| KarmaVLM |  |  |  |  |
| moondream2 |  |  |  |  |

## Details Regarding Models Above📊

### MiniGemini

[![arXiv](https://img.shields.io/badge/arXiv-2403.18814-b31b1b.svg?logo=arXiv)](https://arxiv.org/pdf/2403.18814) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/dvlab-research/MGM)
[![Hugging Face Collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Collections-blue)](https://huggingface.co/collections/YanweiLi/mgm-6603c50b9b43d044171d0854)


##### 动机

为了缩小当前视觉语言模型（VLMs）与先进模型（如GPT-4和Gemini）之间的性能差距，通过挖掘VLMs的潜力，提高其在视觉理解、推理和生成方面的表现。这个动机来源于对VLMs在高分辨率视觉标记、高质量数据和VLM引导生成方面的潜力的探索，以期提升其性能和拓展应用范围。

##### 创新点

主要从下面三个方面挖掘VLM的潜能

1. **High-Resolution Visual Tokens**: Initially, ConvNets are used to generate high-resolution images to enhance image detail. To minimize computational resource expenditure, the author further proposes optimizing for high-resolution without increasing the number of visual tokens, by employing an additional visual encoder.
2. **High-Quality Data**: To bolster data quality, the author amalgamates high-quality datasets from diverse public sources, ensuring a rich and varied foundational dataset.
3. **VLM Guided Generation**: By integrating with a text-to-image model, the capability for image generation is enhanced.

Mini-Gemini supports a series of dense and MoE Large Language Models (LLMs) from 2B to 34B. It is demonstrated to achieve leading performance in several zero-shot benchmarks and even surpasses the developed private models



##### Architecture

<div align="center">
  <img src="./image/minigemini1.png" alt="image-20240510165317066" width="800" />
</div>

<div align="center">
  <img src="./image/minigemini2.png" alt="image-20240510165317066" width="800" />
</div>

In conclusion, dual vision encoders are utilized to provide low-resolution visual embedding and high-resolution candidates; patch info mining is proposed to conduct patch-level mining between high-resolution regions and low-resolution visual queries; LLM is utilized to marry text with images for both comprehension and generation at the same time.

The enhancements are further supported by employing an end-to-end workflow, a dual-resolution visual encoder design for high and low resolution, and a patch info mining module. For detailed information, refer to the paper.



### Bunny

[![arXiv](https://img.shields.io/badge/arXiv-2402.11530-b31b1b.svg?logo=arXiv)](https://arxiv.org/pdf/2402.11530) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/BAAI-DCAI/Bunny)

For more information on the Bunny model checkpoints, please refer to the GitHub link above or click [here](https://github.com/BAAI-DCAI/Bunny). This includes the fully trained checkpoints (for evaluation), the pre-trained checkpoints, and more.

##### 动机

想要beat the scaling law，解决大型MLLM的计算成本问题，通过构建更具信息性的训练数据来训练出性能优越的较小MLLM，从而提高模型的效率和性能。

##### 创新点

该工作 focus on data optimization to compensate for the reduction in model size，并且通过数据集压缩构建了信息量更大的训练数据，即从更广泛的来源中精选数据。

1. **预训练数据集的构建**：整个过程涉及一个精细的三步核心选择方案，基于CLIP嵌入

   - **聚类和图构建**：受SemDeDup方法的启发，他们首先使用k-means算法对所有20亿个图像嵌入进行聚类。在每个簇中，他们创建一个无向图，其中的节点（图像嵌入）在余弦相似度超过预定义阈值（本例中为0.86）时相连。这一步有助于识别相似的图像并减少冗余。
   - **子图过滤**：对于簇中形成的每个连通子图，只保留一个样本 —— 即其到簇质心的欧几里得距离处于中位数的样本。此方法有效地将样本量减少到9.52亿张图像，同时确保每个簇中最具代表性的样本被保留。
   - **基于文本-图像相似度的质量过滤**：然后，他们通过对样本基于每个样本的文本嵌入和对应图像嵌入的余弦相似度进行排序，继续精炼这个子集。通过选择排名在40%到60%之间的样本，他们消除了较低质量的图像-文本对，将数据集规模进一步缩减到1.9亿。
   - **捕捉多样性和本质**：剩余的样本按照每个图像嵌入与其簇质心的余弦相似度进行排序。这里，他们保留排名在15%到35%之间的样本。这一步确保了最终的子集，现在减少到3800万，捕获了原始LAION-2B数据集的本质和多样性。
   - **最终抽样以提高训练效率**：从这个精炼的3800万核心集中，随机抽取200万个样本，形成最终的数据集，命名为Bunny-pretrain-LAION-2M。选择这个规模是为了平衡数据的丰富性与训练的成本和效率。

2. 该工作收集了一组视觉指令微调数据集 — DataOptim1。基于此数据集，他们探索了更好的微调数据集组合。具体而言，他们利用了SVIT-mix-665K [17] 并在其中用WizardLM-evol-instruct-70K [33] 替换了ShareGPT-40K [26]，从而形成了Bunny-695K数据集。

   >他们发现，将多模态学习语言模型（MLLM）在多模态数据上进行微调可能会损害其从预训练语言模型（LLM）继承的认知能力。这可能是由于多模态训练数据中文本信息较少且多样性较低所致。在微调数据集中保留一定量的高质量纯文本数据可以缓解这个问题。

3. 一个即插即用的VLM框架，设计EVA-CLIP 和 SigLIP等视觉编码器和Phi-1.5、StableLM-2 和、Phi-2等大语言模型.

##### Architecture

<div align="center">
  <img src="./image/bunny.png"  width="800" />
</div>
##### Bunny-v1.1🔥

最近推出的Bunny模型！

以SigLIP作为视觉编码器，Phi-3-Mini-4K作为语言编码器。相较于Bunny，其v1.1版本有如下新意：

1. **任务特定标识符**：Bunny-v1.1使用了来自 MiniGPT-v2 的任务特定标识符，这些标识符帮助模型在处理不同类型的任务时进行明确区分。模型使用六个不同的任务标识符，每个标识符对应一个特定的任务，例如视觉问答、图像字幕生成等。
2. **多任务指令模板**：也仿照LLaMA-2 的对话模板设计，包括通用输入格式，如图像特征、任务标识符和指令输入。这种模板设计减少了任务处理过程中的歧义，提高了模型的任务区分能力和执行效率。

### Llava

[![arXiv](https://img.shields.io/badge/arXiv-2304.08485-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2304.08485) 

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/haotian-liu/LLaVA)

作为VLMs领域较为早起的工作，Llava结合了预训练的 CLIP ViT-L/14 视觉编码器和 Vicuna 语言模型，并且通过一个简单的投影矩阵连接两者来实现多模态能力。

创新点

1. Llava使用的也是经典的预训练+微调的训练步骤
2. 创新性地提出了**新的数据集组织方式**，就是利用GPT-4 生成与图像相关的指令问题，例如使用包含了大量的图像及其对应的文本描述的COCO数据集，将图文对儿传输给GPT-4并且组织新的问题，**利用AI产出训练数据来训练AI**。
>为了确保生成的数据具有多样性和深度，研究人员设计了三种不同类型的指令-响应对：
>- 对话式数据（Conversation）： 模拟人与助手之间的对话，涉及关于图像内容的多轮问答。这种类型的数据可以帮助模型学习如何进行连贯的多轮对话。
>- 详细描述（Detailed Description）： 生成详细的图像描述，帮助模型理解和生成详细的视觉内容描述。
> - 复杂推理（Complex Reasoning）： 生成需要复杂推理的问题和答案，涉及多步逻辑推理。这种类型的数据能够提升模型的推理能力。
3. 架构上使用了Flash Attention 2 和 LoRA（低秩自适应）等技术优化，提高效率并减少内存资源的使用

##### Architecture

<div align="center">
  <img src="./image/llava.png"  width="800" />
</div>

##### Llava的改进

The LLaVa model was proposed in [Visual Instruction Tuning](https://arxiv.org/abs/2304.08485) and improved in [Improved Baselines with Visual Instruction Tuning](https://arxiv.org/pdf/2310.03744) by Haotian Liu, Chunyuan Li, Yuheng Li and Yong Jae Lee.这里就是Llava1.5的诞生地

1. **Llava1.5**
   - Llava1.5依旧使用Vicuna 作为基础语言模型，使用了**两层 MLP** 替代了原来的线性投影，同时还支持更高分辨率的图像（336x336 像素）的交互。使用的是划分图像网格的方式，实现了高分辨率输入的处理，这样的方式也巧妙地减少了“幻觉现象”的产生。
   - 引入了面向学术任务的数据集，如VQA（Visual Question Answering）、OCR（Optical Character Recognition）和区域级理解数据
2. **Llava1.6** 🔥
   - 支持更高的像素数（如 672x672, 336x1344, 1344x336 分辨率）图片的交互
   - 添加了视觉推理和 OCR（光学字符识别）能力



### Cog Series

#### CogVLM

[![arXiv](https://img.shields.io/badge/arXiv-2311.03079-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2311.03079) 
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
  <img src="./image/cogVLM.png" alt="image-20240510165317066" width="800" />
</div>




##### 细分

- **CogVLM-Chat**: 模型接受自然语言输入和输出，主要处理纯文本输入和输出，适用于多种VQA和多轮对话数据集
- **CogVLM-Grounding**：侧重于处理包含边界框的输入和输出，支持视觉基准相关的多种任务



##### some tips

LLM是在Vicuna-7B的基础上训练得来的，保证其NLP能力的前提下加上了视觉理解

用到了P-Tuning和LoRA两种高效微调方法



#### CogAgent

[![arXiv](https://img.shields.io/badge/arXiv-2312.08914-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2312.08914) 
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
  <img src="./image/cogAgent.png" alt="image-20240510171107123" width="800" />
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
  <img src="./image/HPT.png"  width="800" />
</div>








### MiniGPT4 Series

Recently, most of the work is based on MiniGPT4 and MiniGPT4-V2. The architectures of MiniGPT4 & MiniGPT4-V2 lay the foundation for subsequent multimodal large models, with subsequent work either adopting their training methods or fine-tuning their entire code structure.

#### MiniGPT4

[![arXiv](https://img.shields.io/badge/arXiv-2304.10592-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2304.10592) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/Vision-CAIR/MiniGPT-4)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-model-blue)](https://huggingface.co/Vision-CAIR/MiniGPT-4)

MiniGPT4总体也是分为视觉端和语言端，包括视觉编码器（ViT 和 Q-Former）和语言模型 Vicuna。使用的是一个简单的线性投影层对齐视觉特征与语言模型。

使用两步训练的方式：

1. 第一阶段使用大量的图像-文本对进行初步训练，获取视觉-语言知识进行**预训练**；经过这一阶段的模型已经可以初步处理一些VQA问题，但是模型有时候还是会输出和提问不相关的内容。
   - 视觉端使用的是ViT 和 Q-Former 
   - 语言端使用的是Vicuna
2. 第二阶段使用高质量高质量的详细图像描述数据集进行**微调**，这一阶段中涉及一个指令数据集，这个数据集的源头是Conceptual Caption数据集，作者使用一阶段训练后的模型生成图片的描述，并且给予足够的提示保证描述足够长，随后使用chatGPT进行进一步的构建和纠错，最后人工选择了3500个左右的图文对作为最后的数据集。



##### Architecture

<div align="center">
  <img src="./image/minigpt4.png"  width="800" />
</div>



#### MiniGPT4-V2

[![arXiv](https://img.shields.io/badge/arXiv-2310.09478-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2310.09478) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/Vision-CAIR/MiniGPT-4)

Minigpt4-v2在MiniGPT4的基础上进行了扩充，主要的创新点和改进如下

1. 使用**任务标识符**区分多模态任务：引入了如[vqa]、[caption]、[grounding]等任务表示符，分别表示视觉问答、图像描述和视觉定位等任务。在训练的时候使用不同下游任务特定的数据集进行微调，同时将任务标识符融入对话模板送入模型，后续在推理的时候人为选择任务标识符告诉gpt完成什么类型的下游任务。这样可以在保证性能的前提下大幅提高模型对下游任务的适配程度，减少幻觉现象和混淆。
2. **三阶段训练策略**
   1. **预训练**：使用弱标注和精细标注的数据集（如LAION、CC3M、SBU、GRIT-20M）训练模型，获取广泛的视觉-语言知识。
   2. **第二阶段：多任务训练**：仅使用精细标注的数据集（如COCO、RefCOCO等）进行多任务训练，优化模型在各个任务上的性能。
   3. **第三阶段：多模态指令调优**：使用多模态指令数据集（如LLaVA、Flickr30k等）和语言数据集（如Unnatural Instructions）进行微调，增强模型的对话能力和指令响应能力。
3. 接受**高分辨率**输入：接受更高分辨率的图像（448x448），并通过将相邻的四个视觉标记拼接成一个标记来减少计算量，提升训练和推理效率。



##### Architecture

<div align="center">
  <img src="./image/minigpt4v2.png"  width="800" />
</div>





### TinyLLaVA

[![arXiv](https://img.shields.io/badge/arXiv-2402.14289-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2402.14289) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/DLCV-BUAA/TinyLLaVABench)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-model-blue)](https://huggingface.co/tinyllava)

TinyLLaVA选择了几个代表性的LLM，包括 TinyLlama（1.1B 参数）、StableLM-2（1.6B 参数）和 Phi-2（2.7B 参数），并且使用 CLIP 和 SigLIP 两种视觉编码器进行最终多模态模型的组装，初步实验发现 SigLIP 与小规模LLM结合效果更好。。

在视觉端和文本端的链接部分，TinyLLaVA使用的是两层多层感知器（MLP）作为视觉编码器和LLM之间的连接器，激活函数为 GELU。

TinyLLaVA参数量虽然比不上一众大模型，但是由于LLM的性能（比如Google的phi-2）足够给力且数据集的质量足够高，使其在多个基准测试中的表现接近甚至超过了一些大规模模型。

##### Architecture 

<div align="center">
  <img src="./image/tinyllava.png"  width="800" />
</div>


### TinyGPT-V 
[![arXiv](https://img.shields.io/badge/arXiv-2312.16862-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2312.16862) 

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/DLYuanGod/TinyGPT-V)

[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-model-blue)](https://huggingface.co/Tyrannosaurus/TinyGPT-V)

TinyGPT-V 也是在探究如何使用小型Backbone实现多模态大型语言模型，模型总体依旧是分为视觉端、语言端和映射层，语言端使用的是Phi-2，视觉端使用的是预训练的EVA（Enhanced Vision Attention）ViT（Vision Transformer）模型，映射层采用BLIP-2架构中的Q-Former层作为初始映射层，利用BLIP系统的预训练优势。总体来说可以将TinyGPT-V 的创新与亮点归纳为以下几点：

1. **视觉-语言映射层的结构**：TinyGPT-V 的视觉-语言映射层组合了多个小模块，这些模块来自不同模型（包括视觉模型、其他VLM等），可以分成三个主要层次（详细设计见[下图](#train process)）：

   - **Q-Former层（初始映射层）**：来自BLIP-2架构的Q-Former层作为初始映射层，希望使用这样一个预训练得当且表现很好的结构作为视觉-语言对齐的初始结构，有效地将视觉编码器（EVA ViT）提取的高维度视觉特征转换为适合语言模型处理的表示。
   - **第一层线性投影**：采用来自MiniGPT-4的预训练线性投影层，这样可以适当加快训练过程，因为MiniGPT-4的预训练线性投影层已经包含了丰富的模式和特征，可以直接使用不用重头训练。
   - **第二层线性投影**：通过高斯分布初始化的新线性投影层，确保特征最终整合到Phi-2模型的隐藏空间中。

2. **四阶段训练策略**：

   - **阶段1：热身训练**： 使用大规模图像-文本对数据集（如LAION、Conceptual Captions、SBU）进行初始预训练。用上述数据集进行初步训练，模型识别投影层的输出作为软提示（soft prompt），指导其生成相关文本。（使用共计约500万对图像-文本对）。
   - **阶段2：再预训练**： 专门训练LoRA模块，进一步减少图像-文本对的损失。此阶段的训练目的是使LoRA模块在处理多模态数据时发挥作用，提高模型的学习能力和性能。
   - **阶段3：指令微调**： 使用MiniGPT-4或LLaVA的数据集进行指令微调，提高模型生成一致且自然响应的能力。
   - **阶段4：多任务学习**： 通过多模态指令数据集（如LLaVA、Flickr30k）进行多任务学习，提高模型在多轮对话中的任务处理能力。

3. **规范化与LoRA**：作者还发现小型大规模语言模型在进行迁移的时候有很多弊端需要克服。small VLM由于参数较少，在数据计算中对NaN或INF值比较敏感，这将导致初始批前向传播失败。TinyGPT-V使用了多样的归一化技巧解决这些问题：

   - **RMSNorm（RMS归一化）**：RMSNorm用于解决梯度消失或爆炸的问题，确保模型在训练过程中的稳定性。具体而言，RMSNorm在每个多头注意力层（MHA）之后应用，以规范化数据。【下面公式中，x~post~是MHA后的输入，N是 ~post~ 的维度。】
     $$
     \text{RMSNorm}(x_{\text{post}}) = \frac{x_{\text{post}}}{\sqrt{\frac{1}{N} \sum_{i=1}^{N} x_i^2 + \epsilon}}
     $$

   - **Query-Key Normalization（查询-键归一化）**：Query-Key Normalization在低资源学习场景中特别有效，帮助模型在处理多模态数据时保持计算的稳定性。【下面公式中，d~k~ 表示Q或K的维度。】
     $$
     \text{Attention}(Q, K, V) = \text{softmax}\left(\frac{\text{LayerNorm}(Q) \cdot \text{LayerNorm}(K)^T}{\sqrt{d_k}}\right) V
     $$

   - **Layer Normalization（层归一化）**：在每一层中应用Layer Normalization，通过标准化输入来防止NaN值的产生。【下面公式中，其中，x~hidden~ 是该层的输入，*μ* 和 *σ*^2^ 分别是输入的均值和方差，*γ* 和 *β* 是可训练的参数。】
     $$
     \text{LayerNorm}_{\text{input}}(x_{\text{hidden}}) = \gamma \frac{x_{\text{hidden}} - \mu}{\sqrt{\sigma^2 + \epsilon}} + \beta
     $$

   -  **LoRA（Low-Rank Adaptation）**：LoRA通过在冻结预训练权重的情况下引入低秩矩阵进行参数高效微调，减少训练时的参数调整量，避免梯度消失。

4. **任务特定标识符与指令模板**：类似于MiniGPT4和MiniGPT-v2，TinyGPT-V 也在指令模板中融入了任务特定标识符，这样可以提高模型在多任务和多轮对话中的表现。TinyGPT-V利用从MiniGPT-v2中借鉴的多任务指令模板，总体而言的修改并不多，**在空间位置识别方面有一些改进**。具体来说，对于需要识别引用对象空间位置的任务，TinyGPT-V使用文本表示的边界框，并将坐标归一化到0到100之间。除了这个改进以外其他的没有提及。

   

##### Architecture

<div align="center">
  <img src="./image/TinyGPT-V.png"  width="800" />
</div>


##### Train process
<div align="center">
  <img src="./image/Training_S.png"  width="800" />
</div>



### PaLI-3
[![arXiv](https://img.shields.io/badge/arXiv-2310.09199-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2310.09199) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/google-research/big_vision)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-model-blue)](https://huggingface.co/tinyllava)

PaLI-3，这是 PaLI 系列的第三代模型。通过一个仅有 5B 参数的预训练基线模型，他们优化了训练方法，并在多个 VLM 基准上实现了有竞争力以及新的 SOTA 结果。

新的方法主要由三个步骤：

1. **单模态预训练**：预训练图像编码器和文本编码器，使它们能够单独处理各自的输入。

   - **图像编码器预训练**：使用网页规模的图像-文本对数据集（如 WebLI）。采用 SigLIP 训练方法，对图像和文本进行对比预训练

     >1. **嵌入**：将图像和文本嵌入到同一高维向量空间中。
     >2. **对比损失**：使用 Sigmoid Cross-Entropy 损失函数，使正确的图像-文本对的点积较高，而不正确的对较低。

   - **文本编码器预训练**：使用 UL2 模型，采用“去噪器混合”（mixture of denoisers）的方法进行训练。

2. **多模态训练**

   - 将预训练的图像编码器（ViT-G/142）与一个 3B 参数的 UL2 编码器-解码器语言模型结合。图像编码器将图像转换为视觉令牌，这些令牌与文本令牌一起输入到语言模型中。
   - 在这个阶段，**图像编码器保持冻结状态，只训练语言模型部分**，以确保图像编码器的嵌入质量。
   - **高分辨率训练**:开始时使用较低分辨率的图像，逐步提高分辨率，以提高模型对图像细节的感知能力。中间会在 812×812 和 1064×1064 分辨率上保存检查点。

3. **分辨率增加和任务专用微调**:

   - 进一步提高模型的输入分辨率，进行短期微调，解冻图像编码器，确保模型能够在高分辨率下处理图像。
   - **任务专用微调**：在微调过程中，通常使用 812×812 分辨率检查点，但对于某些需要更高分辨率的任务（如文档理解任务），会使用 1064×1064 分辨率进行微调。

##### Architecture

<div align="center">
  <img src="./image/paligemma.png"  width="800" />
</div>


### PaliGemma

[![AI Blog](https://img.shields.io/badge/AI%20Blog-PaliGemma%20AI-orange.svg)](https://ai.google.dev/gemma/docs/paligemma) 

[![AI Blog](https://img.shields.io/badge/AI%20Blog-paligemma%20AI-orange.svg)](https://huggingface.co/blog/paligemma) 

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/google-research/big_vision)


PaliGemma 由 [Transformer 解码器](https://arxiv.org/abs/1706.03762)和 [Vision Transformer 图像编码器](https://arxiv.org/abs/2010.11929)组成，共计有 30 亿个参数。文本解码器从 [Gemma-2B](https://www.kaggle.com/models/google/gemma) 初始化。图片编码器使用 [SigLIP-So400m/14](https://colab.research.google.com/github/google-research/big_vision/blob/main/big_vision/configs/proj/image_text/SigLIP_demo.ipynb?hl=zh-cn) 进行初始化。PaliGemma 是按照 PaLI-3 方法训练的。

PaliGemma 共开源了三类模型：
（1）预训练的多模态基座模型（模型在huggingface上标注为pt）；
（2）在单个任务上（如：DocVQA，AI2D 等）Finetune 得到的模型（模型在huggingface上标注为ft）；
（3）混合数据集上 Finetune 的模型（模型在huggingface上标注为mix）。

这些模型有三种不同的分辨率（224x224、448x448）、896x896和三种不同的精度 （bf16、f16和f32）。每个存储库都包含给定分辨率和任务的检查点，每个可用精度都有三个修订版。每个存储库的main分支都包含float32检查点，其中bf16as 和f16revisions 包含相应的精度。对于与 Transformer 和原始 JAX 实现兼容的模型，有单独的存储库，高分辨率模型需要更大的内存来运行，因为输入序列要长得多。它们可能有助于处理颗粒度较为精细的任务（如 OCR），但对于大多数任务来说，质量提升很小。

##### Architecture

same as [PaLI-3](#palI-3)

<div align="center">
  <img src="./image/paligemma.png"  width="800" />
</div>
### MobileVLM

#### MobileVLM(base)

[![arXiv](https://img.shields.io/badge/Arxiv-2312.16886-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2312.16886) 

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/Meituan-AutoML/MobileVLM)

MobileVLM是首个专门为移动和物联网设备设计的多模态视觉语言模型，视觉端使用的是CLIP ViT-L/14@336 ，语言端使用的是MobileLLaMA ，连接视觉与语言的投影层是一个有着独特设计的网络结构。MobileVLM主要的特点有以下几个方面

1. **轻量化下采样投影器（LDP）**：通过减少视觉tokens的数量，提高多模态特征的对齐效率，同时降低计算开销。（详细设计见[下图](#architecture-13)）
   - 使用**深度卷积**（Depthwise Convolution）和**逐点卷积**（Pointwise Convolution）相结合的方式。用深度卷积用于捕获局部空间特征，而逐点卷积用于特征压缩和特征对齐。
   - **高效的下采样策略**：采用步长为2的卷积操作来实现视觉特征的下采样，将视觉tokens数量减少75%。有效地保留了关键视觉信息，同时大幅减少了需要处理的tokens数量
   - **使用层归一化**（Layer Normalization）代替批归一化（Batch Normalization），以确保训练稳定且不受批量大小的影响。
   - **多层次的特征交互**：在卷积层前后添加逐点卷积层，实现了特征空间和token之间的多层次交互。
2. **全栈重制多模态视觉语言模型**：MobileVLM是一个从头开始构建的专门针对移动设备优化的多模态模型，详细的训练流程如下
   - **基础语言模型的预训练**：使用RedPajama v1数据集（包含1.3万亿个token）训练LLM，LLM选择的是基于LLaMA的24层和32层的变体，分别具有1.4B和2.7B参数。
   - **监督微调（Supervised Fine-Tuning, SFT）**：使用的是基于Vicuna的多轮对话数据集（包括用户与ChatGPT的对话记录）
   - **多模态模型训练（Training of Multimodal Models）**：使用CC-595K和LLaVA-Instruct-158K数据集进行预训练和指令微调。
     - **预训练（Pre-training）**：冻结视觉编码器和语言模型，仅训练轻量化下采样投影器（LDP）。
     - **指令微调（Instruction Tuning）**：微调投影器和语言模型，增强视觉理解和表达能力。

3. **低秩适应（LoRA）**：视觉指令微调阶段应用LoRA，仅更新8.87%和7.41%的LLM参数，就能实现与完全微调相媲美的性能
4. **消融实验**：针对新提出的LDP还进行了相关消融实验，对比了传统的减少分辨率的方法和轻量化下采样投影器（LDP）方法，结果显示LDP）能够减少75%的视觉tokens数量（从576减少到144），并最终实现与基线相当甚至更好的性能，这表明在减少tokens数量的同时，视觉tokens的质量得到了进一步提升。



##### Architecture

<div align="center">
  <img src="./image/mobilellava.png"  width="800" />
</div>




#### MobileVLM V2

[![arXiv](https://img.shields.io/badge/Arxiv-2402.03766-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2402.03766)

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/Meituan-AutoML/MobileVLM)

MobileVLM V2继续在低资源的VLM领域探索方向，相比MobileVLM，v2版本有以下几方面的改进：

1. **增强的训练数据**：

   - MobileVLMv2在预训练阶段使用了来自ShareGPT4V的120万高质量图文对齐数据，数据质量的提升提高了训练效率和模型性能

     > ShareGPT4V数据集是从GPT-4V（Vision）生成的，这些模型本身已经经过大量高质量数据的训练，能够生成准确且详细的图文对齐数据。而且ShareGPT4V数据集涵盖了多个领域和场景，**还经过细致的标注**，这种广泛的覆盖和标注的准确性有助于模型在不同任务中表现良好。

   - 还引入了多个学术任务数据集，如ScienceQA、TextVQA和SBU，增加了数据的多样性和指令跟随能力。

2. **优化了投影器的结构**：新的投影器包含三个组件——特征转换、token 减少和位置信息增强。

   - **特征转换**：使用两个逐点卷积层（Pointwise Convolution）对图像tokens进行特征转换，使其特征维度与大语言模型（LLM）匹配。
   - **token 减少**：引入平均池化层（Average Pooling）对图像tokens进行大幅压缩。具体操作为使用2×2的平均池化层，将图像tokens数量减少到原来的1/4。
   - **位置信息增强**：应用了一个简单但有效的模块 PEG（Position Encoding Generator），并使用skip connection（跳跃连接）增强位置信息。这种方法显著减少了参数数量，同时略微提升了运行速度。

3. **新的训练策略**：

   - **预训练**：
     - **初始化**：视觉端使用预训练的CLIP ViT-L/14模型权重。语言端使用预训练的MobileLLaMA模型权重。投影器参数为随机初始化
     - **活动与冻结**：冻结视觉编码器，仅训练投影器和语言模型，使得模型的训练目标集中在预测下一个token上。
   - **多任务训练和微调**：本工作引入了多个视觉-语言相关的下游任务，**解冻并训练所有组件，包括投影器和语言模型**。
     - Visual Dialog：123K 样本
     - Text-VQA：35K 样本
     - VSR：13K 样本
     - VIGC：37K 样本
     - IConQA：107K 样本
     - SQA：13K 样本
     - COCO：592K 样本
     - SBU：844K 样本
     - ShareGPT4V：665K 样本
     - **总样本数**：360万个样本



##### Architecture

<div align="center">
  <img src="./image/MobileVLMV2.png"  width="800" />
</div>

### LLaVA-Phi

[![arXiv](https://img.shields.io/badge/Arxiv-2401.02330-b31b1b.svg?logo=arXiv)](https://arxiv.org/pdf/2401.02330)

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/zhuyiche/llava-phi)

LLaVA-Phi（也称作LLaVA-φ）是组合了两个视觉端和语言端的小模型组成的多模态小模型，将LLava中的vicuna换成了phi实现了很多benchmark的SOTA。LLaVA-Phi接受336x336尺寸的图片（用的是分辨率为336*336的预训练CLIP ViT-L/14），以两层MLP作为视觉端和语言端的链接部分。

LLaVA-Phi还真对phi-2进行了微调，使用类似Vicuna 格式组织指令模板进行微调。

**具体的两阶段训练策略**：

- **预训练阶段**：使用 CC-595K 数据集的过滤子集进行一轮预训练，学习率为 1e-3，批次大小为 256。
- **指令微调阶段**：在 LLaVA-Instruct-150K 数据集上进行一轮微调，学习率为 2e-5，批次大小为 256。微调过程中使用 Adam 优化器，权重衰减为 0.1，动量参数为 0.9 和 0.98，epsilon 值为 1e-7。



### LLaVA-Phi-3-mini

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/InternLM/xtuner)

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/xtuner/llava-phi-3-mini-662a5f7b9416630a1ad91102)

LLaVA-Phi-3-Mini系列模型是在 LLaVA-Phi 基础上进一步微调的，使用了 Phi-3-mini 和 CLIP-ViT-Large-patch14-336，结合了 ShareGPT4V-PT 和 InternVL-SFT 数据集进行训练，还支持多种量化。



### IMP

[![arXiv](https://img.shields.io/badge/arXiv-2405.12107-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2405.12107) 

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/MILVLG/imp)

[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-model-blue)](https://huggingface.co/MILVLG/imp-v1-3b)

IMP is build upon a small yet powerful SLM [Phi-2](https://huggingface.co/microsoft/phi-2) (2.7B) and a powerful visual encoder [SigLIP](https://huggingface.co/google/siglip-so400m-patch14-384) (0.4B), and trained on the [LLaVA-v1.5](https://github.com/haotian-liu/LLaVA) training set.`imp-v1-3b`

在 Qualcomm Snapdragon 8Gen3 移动芯片上实现了每秒约 13 个 tokens 的高推理速度，使得模型在移动设备上高效运行。

**两阶段训练策略**：

- **第一阶段：多模态对齐预训练**。仅训练多模态连接器，同时冻结视觉编码器和语言模型。
- **第二阶段：多模态指令微调**。同时优化语言模型和多模态连接器，增强模型的指令跟随能力。

**模型架构优化**：

- 通过选择合适的语言模型和视觉编码器，并进行优化，提升了模型的整体性能和效率。

**训练策略改进**：

- 采用 LoRA（低秩适应）微调机制和优化的训练轮数，确保模型在有限资源下达到最佳性能。

**数据增强**：

- 引入 OCR 和图表数据、GPT4V 注释数据等，丰富了训练数据的多样性和质量，提升了模型的泛化能力。

🔥IMP最近推出了[Imp-v1.5](https://huggingface.co/collections/MILVLG/imp-v15-664c07c27a71afa504f69cec)系列模型。包括 Imp-v1.5-2B、Imp-v1.5-3B 和 Imp-v1.5-4B，进一步扩展了 Imp 模型的能力范围。



### MoE-LLaVA
[![arXiv](https://img.shields.io/badge/arXiv-2401.15947-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2401.15947) 

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/PKU-YuanGroup/MoE-LLaVA)

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/LanguageBind/moe-llava-model-65b607bf2524ac36e733874c)



MoE-LLaVA也是基于MoE（混合专家模型）的VLM，该VLM结合多个专家模型（专家网络）以增强其多模态能力和泛化性能。但是对于大型的VLM，参数的提升虽然可以带来性能的增强，但是训练和推理所需的计算资源也迅速增加，该工作就解决了这个方面的问题。

##### 动机

为了在有限的计算资源上训练高性能的VLM，来自北京大学、中山大学等机构发布的MoE-LLaVA提出了一种巧妙而新颖的叫做MoE-Tuning的训练策略，可以实现参数量大的同时保证其所需的计算资源恒定。

##### 创新点

1. **三阶段的基于MoE-Tuning的训练策略**（图示参见[link](#train process-2)）

   - **阶段 I: 适应视觉输入**：主要目标是将图像token适应LLM，使得LLM能够理解图像中的实例
     - 使用一个多层感知机（MLP）将图像token投影到LLM的输入域中，将图像块视为伪文本token。
     - 在这个阶段，仅训练MLP层，而不训练LLM的其他参数。
   - **阶段 II——增强多模态理解能力**：目标是通过多模态指令数据的调优，使LLM具备多模态理解能力。
     - 解冻并训练LLM的所有参数，增强其处理多模态数据的能力。
     - 使用包含复杂任务的多模态指令数据进行训练，如图像逻辑推理和文本识别，这些任务要求模型具备更强的多模态理解能力。
     - 在这个阶段完成后，LVLM已具备初步的多模态理解能力，为下一阶段的稀疏化打下基础。
   - **阶段 III——引入MoE层的稀疏化**：目标是通过引入稀疏化机制，使模型在保持高性能的同时降低计算成本，具体来说有以下几个步骤：
     - **初始化专家权重**：将阶段II中的FFN权重复制为每个专家的初始化权重。
     - **训练MoE层**：仅训练MoE层，确保每个token由前k个概率最高的专家处理，其余专家保持不活动状态。
     - **路由器计算权重**：使用线性层路由器预测每个token分配给每个专家的概率，并根据软最大值函数进行归一化。每个token由前k个专家处理，并基于路由器权重进行加权求和。

2. **基于MoE的稀疏LVLM架构**

   - 起初，图像通过视觉编码器处理得到视觉token序列Z，文本通过词嵌入层处理得到文本token序列T，视觉token和文本token拼接成一个序列，并作为LLM的输入。
   - 随后，在模型的前向传播过程中，在每个MoE层中，路由器计算每个token被分配到每个专家的概率，选择前k个专家进行处理，并通过加权求和得到最终输出。
   - 实现了在保持计算成本不变的情况下显著扩展模型参数数量

3. **MoE层工作机制和FFN细节**：MoE层引入多个专家（每个专家都是一个独立的FFN）并动态选择最适合处理当前输入的专家，以此提升模型性能

   - **初始化**：在第三阶段训练策略中，FFN的权重被复制并初始化为多个专家的权重。这些专家组成一个集合E = [e1, e2, ..., eE]
   - **路由器计算权重**：路由器是一个线性层，它接收输入token并生成每个专家的权重logits，进随后权重经过softmax归一化后得到选择每个专家的概率
   - **选择专家**：选择前k个概率最高的专家进行处理，这些被选择的专家称为“激活专家”。
   - **专家处理**：每个激活专家对输入token进行处理，计算得到输出，激活专家的输出通过加权求和得到最终的MoE层输出

   > 未被选中的专家保持不活动状态，不参与计算，从而减少了计算开销。

   



##### Architecture

<div align="center">
  <img src="./image/moe-llava.png"  width="800" />
</div>

架构总体包含以下组件

1. **视觉编码器（Vision Encoder）**：
   - 输入RGB图像，将其处理为视觉token序列。图像的原始分辨率为H×W，视觉编码器将其转化为P个视觉token，每个token的维度为C。
2. **视觉投影层（Visual Projection Layer, MLP）**：
   - 将视觉token序列从维度C映射到LLM的隐藏尺寸D。
3. **词嵌入层（Word Embedding Layer）**：
   - 将文本token投影到LLM的隐藏尺寸D。
4. **大语言模型（LLM）**：
   - 由多个堆叠的多头自注意力（MSA）层和前馈神经网络（FFN）层组成，层归一化（LN）和残差连接应用于每个块。
5. **MoE层**：
   - 由多个FFN专家组成，每个token通过可学习的路由器分配给前k个专家，未被激活的专家保持不活动状态。

##### Train process

<div align="center">
  <img src="./image/moe-llava-train.png"  width="800" />
</div>


### Cobra

[![arXiv](https://img.shields.io/badge/arXiv-2403.14520-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2403.14520) 

[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/h-zhao1997/cobra)

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/han1997/cobra-6615c3242851ba108027105d)

Cobra多模态大模型是由西湖大学和浙江大学联合推出的一个研究项目，结合了[Mamba](./README.md#mamba)语言模型




## something else

最新的VLMs survey存储库，包括VLM预训练、迁移学习方法和知识蒸馏方法，还有可以使用的数据集汇总：[github](https://github.com/jingyi0000/VLM_survey)

## Response time

The GitHub project [fastestAI]([fastai/fastai: The fastai deep learning library (github.com)](https://github.com/fastai/fastai)) has compiled response time data for recently released LLMs (Large Language Models) and VLMs (Vision Language Models). For detailed statistics, please refer to the table available at this [link](https://thefastest.ai).

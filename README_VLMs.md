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
|    HPT     |       3-8B/6B | NONE |            [HPT](https://huggingface.co/HyperGAI)            |    [HPT](#hpt)    |
| MiniGPT4 Series | 7B/13B | Invalid Now | [Vision-CAIR ](https://huggingface.co/Vision-CAIR) | [MiniGPT4 Series](#minigpt4-series) |
| TinyLLaVA | 1.4B/2.4B/3.1B | NONE | [TinyLLaVA](https://huggingface.co/tinyllava) | [TinyLLaVA](#tinyllava) |
| TinyGPT-V |  | | [TinyGPT-V]() | [TinyGPT-V](#tinygpt-v) |
| PaliGemma | 3B | [PaliGemma](https://huggingface.co/spaces/big-vision/paligemma) | [PaliGemma Family](https://huggingface.co/collections/google/paligemma-ft-models-6643b03efb769dad650d2dda) | [PaliGemma](#paligemma) |
| PaLI-3 | 5B |  |  | [PaLI-3](#palI-3) |

## Details Regarding Models Above📊

### MiniGemini

[![arXiv](https://img.shields.io/badge/arXiv-2403.18814-b31b1b.svg)](https://arxiv.org/pdf/2403.18814) 
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
  <img src="./image/minigemini1.png" alt="image-20240510165317066" width="600" />
</div>

<div align="center">
  <img src="./image/minigemini2.png" alt="image-20240510165317066" width="600" />
</div>

In conclusion, dual vision encoders are utilized to provide low-resolution visual embedding and high-resolution candidates; patch info mining is proposed to conduct patch-level mining between high-resolution regions and low-resolution visual queries; LLM is utilized to marry text with images for both comprehension and generation at the same time.

The enhancements are further supported by employing an end-to-end workflow, a dual-resolution visual encoder design for high and low resolution, and a patch info mining module. For detailed information, refer to the paper.



### Bunny

[![arXiv](https://img.shields.io/badge/arXiv-2402.11530-b31b1b.svg)](https://arxiv.org/pdf/2402.11530) 
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
  <img src="./image/bunny.png"  width="600" />
</div>


### Llava

[![arXiv](https://img.shields.io/badge/arXiv-2304.08485-b31b1b.svg)](https://arxiv.org/abs/2304.08485) 

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
  <img src="./image/llava.png"  width="600" />
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



### MiniGPT4 Series

#### MiniGPT4



#### MiniGPT4-V2





### TinyLLaVA

[![arXiv](https://img.shields.io/badge/arXiv-2402.14289-b31b1b.svg)](https://arxiv.org/abs/2402.14289) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/DLCV-BUAA/TinyLLaVABench)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-model-blue)](https://huggingface.co/tinyllava)







### TinyGPT-V  



### PaLI-3

[[2310.09199\] PaLI-3 Vision Language Models: Smaller, Faster, Stronger (arxiv.org)](https://arxiv.org/abs/2310.09199)

[google-research/big_vision: Official codebase used to develop Vision Transformer, SigLIP, MLP-Mixer, LiT and more. (github.com)](https://github.com/google-research/big_vision?tab=readme-ov-file)

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
  <img src="./image/paligemma.png"  width="600" />
</div>





### PaliGemma

[PaliGemma  | Google for Developers](https://ai.google.dev/gemma/docs/paligemma?hl=zh-cn)

[PaliGemma – Google's Cutting-Edge Open Vision Language Model (huggingface.co)](https://huggingface.co/blog/paligemma)

[PaliGemma](https://github.com/google-research/big_vision)

PaliGemma 由 [Transformer 解码器](https://arxiv.org/abs/1706.03762)和 [Vision Transformer 图像编码器](https://arxiv.org/abs/2010.11929)组成，共计有 30 亿个参数。文本解码器从 [Gemma-2B](https://www.kaggle.com/models/google/gemma) 初始化。图片编码器使用 [SigLIP-So400m/14](https://colab.research.google.com/github/google-research/big_vision/blob/main/big_vision/configs/proj/image_text/SigLIP_demo.ipynb?hl=zh-cn) 进行初始化。PaliGemma 是按照 PaLI-3 方法训练的。

PaliGemma 共开源了三类模型：
（1）预训练的多模态基座模型（模型在huggingface上标注为pt）；
（2）在单个任务上（如：DocVQA，AI2D 等）Finetune 得到的模型（模型在huggingface上标注为ft）；
（3）混合数据集上 Finetune 的模型（模型在huggingface上标注为mix）。

这些模型有三种不同的分辨率（224x224、448x448）、896x896和三种不同的精度 （bf16、f16和f32）。每个存储库都包含给定分辨率和任务的检查点，每个可用精度都有三个修订版。每个存储库的main分支都包含float32检查点，其中bf16as 和f16revisions 包含相应的精度。对于与 Transformer 和原始 JAX 实现兼容的模型，有单独的存储库，高分辨率模型需要更大的内存来运行，因为输入序列要长得多。它们可能有助于处理颗粒度较为精细的任务（如 OCR），但对于大多数任务来说，质量提升很小。

##### Architecture

same as [PaLI-3](#palI-3)

<div align="center">
  <img src="./image/paligemma.png"  width="600" />
</div>




## Response time

The GitHub project [fastestAI]([fastai/fastai: The fastai deep learning library (github.com)](https://github.com/fastai/fastai)) has compiled response time data for recently released LLMs (Large Language Models) and VLMs (Vision Language Models). For detailed statistics, please refer to the table available at this [link](https://thefastest.ai).

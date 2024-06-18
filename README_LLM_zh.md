<div align="center">
  <img src="./image/title.png" width="800" />
</div>
<div align="center">
 <strong>🌐✨关于近期的🔥LLMs🔥的github Awesome List</strong><br>
<strong>中文</strong> | <strong><a href="./README_LLM.md">English🚀</a></strong><br>
<strong>LLMs</strong> | <strong><a href="./README_VLMs.md">VLMs🚀</a></strong>
</div>
## 近期LLM概览

<div align="center">
  <img src="./image/LLM2023.png"  width="800" />
</div>
<div align="center">
  <img src="./image/LLM2024.png"  width="800" />
</div>
*<em>图片来源: <a href="https://lifearchitect.ai/models">LifeArchitect.ai/models</a></em>*

## 快速开始🏁

|    模型   |     发行方   |        参数规模        |                          模型检查点                          |            详细介绍            |
| :----------: | :-------------------: | :----------------------: | :----------------------------------------------------------: | :---------------------------: |
| ChatGPT | OpenAI | --- | --- | [Hyperlink](#chatgpt) |
|   Llama 2    |         Meta          |        7B/13B/70B        | [Llama2 Family🤗](https://huggingface.co/collections/meta-llama/llama-2-family-661da1f90a9d678b6f55773b) |     [Hyperlink](#llama2)      |
|   Llama 3    |         Meta          |          8B/70B          | [Llama3 Family🤗](https://huggingface.co/collections/meta-llama/meta-llama-3-66214712577ca38149ebb2b6) |     [Hyperlink](#llama3)      |
|    Orca2     |       Microsoft       |          7B/13B          | [Orca Family🤗](https://huggingface.co/collections/microsoft/orca-65bbeef1980f5719cccc89a3) |      [Hyperlink](#orca2)      |
|     Qwen     |        Alibaba        | 0.5B/1.8B/4B/7B/14B/72B  |             [Qwen🤗](https://huggingface.co/Qwen)             |         [Hyperlink](#qwen)         |
|   Qwen1.5    |        Alibaba        | 0.5B/1.8B/4B/7B/14B/72B  |           [Qwen1.5🤗](https://huggingface.co/Qwen)            |      [Hyperlink](#qwen15)       |
|    Vicuna    |         LMSYS         |        7B/13B/33B        |           [Vicuna🤗](https://huggingface.co/lmsys)            |       [Hyperlink](#vicuna)       |
|     XGen     |      Salesforce       |            7B            | [xgen-7b-4k-base🤗](https://huggingface.co/Salesforce/xgen-7b-4k-base) |         [Hyperlink](#xgen)         |
|    Falcon    |          UAE          |    1.3B/7.5B/40B/180B    | [Falcon Family🤗](https://huggingface.co/collections/tiiuae/falcon-64fb432660017eeec9837b5a) |       [Hyperlink](#falcon)       |
|     phi      |       Microsoft       |        1B/1.5B/2B        | [phi-1B🤗](https://huggingface.co/microsoft/phi-1)<br />[phi-1.5B🤗](https://huggingface.co/microsoft/phi-1_5)<br />[phi-2B🤗](https://huggingface.co/microsoft/phi-2) |          [Hyperlink](#phi)          |
|     phi3     |       Microsoft       |       3.8B/7B/14B        | [Phi-3 family🤗 **(only phi-3-mini is available now)**](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3) |         [Hyperlink](#phi3)         |
|    Gemma     |        Google         |          2B/7B           | [Gemma Family🤗](https://huggingface.co/collections/google/gemma-release-65d5efbccdbb8c4202ec078b) |        [Hyperlink](#gemma)        |
|    Mamba     | Albert Gu and Tri Dao | 130M/370M/790M/1.4B/2.8B |     [state-spaces🤗](https://huggingface.co/state-spaces)     |        [Hyperlink](#mamba)        |
|    Pythia    |      EleutherAI       |         14M～12B         | [Pythia Family🤗](https://huggingface.co/collections/EleutherAI/pythia-scaling-suite-64fb5dfa8c21ebb3db7ad2e1) |       [Hyperlink](pythia)        |
|   Mistral    |      Mistral AI       |            7B            |         [Mistral🤗](https://huggingface.co/mistralai)         |      [Hyperlink](#Mistral)      |
|      YI      |         01-ai         |        6B/9B/34B         | [Yi Family](https://huggingface.co/collections/01-ai/yi-2023-11-663f3f19119ff712e176720f) |           [Hyperlink](#yi)           |
|    YI-1.5    |         01-ai         |        6B/9B/34B         | [Yi-1.5 Family🤗](https://huggingface.co/collections/01-ai/yi-15-2024-05-663f3ecab5f815a3eaca7ca8) |       [Hyperlink](#yi-15)        |
|    Zephyr    |     Hugging Face      |            7B            |   [HuggingFaceH4🤗 ](https://huggingface.co/HuggingFaceH4)    |       [Hyperlink](#zephyr)       |
| StripedHyena |      Together AI      |            7B            | [StripedHyena Family🤗](https://huggingface.co/collections/togethercomputer/stripedhyena-65d8e6e77540dd1da932dbe1) | [Hyperlink](#stripedHyena) |
|  Persimmon   |     Adept AI Labs     |            8B            | [persimmon-8b-chat🤗](https://huggingface.co/adept/persimmon-8b-chat) |    [Hyperlink](#persimmon)    |



## 模型细节📊

### ChatGPT

OpenAI最近发布了一个实用的用于LLM评估的库[[GitHub]](https://github.com/openai/simple-evals)，目的是确保他们发布的模型准确性数据的透明度，例如GPT-4-turbo。涉及MMLU、MATH、GPQA、DROP、MGSM、HumanEval等Benchmark。



### Llama2

[![arXiv](https://img.shields.io/badge/arXiv-2307.09288-b31b1b.svg)](https://arxiv.org/abs/2307.09288) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/meta-llama/llama)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/meta-llama/llama-2-family-661da1f90a9d678b6f55773b)


Llama 2预训练模型相较于 Llama 1 模型有显著提升，增加了 40% 的训练词元总数，并采用了更长的上下文长度（高达 4000 词元），同时还利用分组查询注意力机制，极大加速了 70B 模型的推理速度。Llama 2-Chat 系列模型采用了基于人类反馈的强化学习（RLHF）技术，专门针对对话场景进行优化。在广泛的有用性和安全性测试基准中，Llama 2-Chat 的表现超过了多数现有开放模型，并且在人类评估中显示出与 ChatGPT 相媲美的性能。

- **Date:** 2023-07
- **Pretrain Data Scale:** 2T
- **Language Support:** en
- **Parameter Size:** 7B/13B/70B



### Llama3

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Meta%20AI-orange.svg)](https://ai.meta.com/blog/)
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/meta-llama/llama3)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/meta-llama/meta-llama-3-66214712577ca38149ebb2b6)

相较于 Llama 2，Llama 3 最显著的变化在于引入了一个新的 Tokenizer，并将词汇表的规模扩展到了 128,256 个词汇（先前版本为 32,000 个 Token）。这样一个更庞大的词汇表可以更有效地对文本进行编码，无论是输入还是输出，也可能增强模型处理多语言的能力。然而，这一改变同时导致了嵌入层的输入和输出矩阵的尺寸增大，从而增加了小型模型的参数量。

- **Date:** 2024-04
- **Pretrain Data Scale:** 1.5T
- **Language Support:** en
- **Parameter Size:** 8B/70B



### Orca2
[![arXiv](https://img.shields.io/badge/arXiv-2311.11045-b31b1b.svg)](https://arxiv.org/pdf/2311.11045.pdf) 
[![Hugging Face collection](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/microsoft/orca-65bbeef1980f5719cccc89a3)


Orca 2 is a finetuned version of LLAMA-2. Orca 2’s training data is a synthetic dataset that was created to enhance the small model’s reasoning abilities. All synthetic training data was moderated using the Microsoft Azure content filters.

论文中详细介绍了Orca 是如何在较小模型的情况下，也能媲美 GPT 3.5 甚至 GPT 4 的大语言模型。

- **Date:** 2023-11
- **Pretrain Data Scale:** same as LLAMA-2
- **Language Support:** en
- **Parameter Size:** 7B/13B



### Qwen

[![arXiv](https://img.shields.io/badge/arXiv-2309.16609-b31b1b.svg)](https://arxiv.org/abs/2309.16609) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/QwenLM/Qwen) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/Qwen)

通过指令微调（Instruction Fine-Tuning）对特定任务进行优化，比如编程语言生成（CodeQwen），采用了混合专家（Mixture of Experts, MoE）和稀疏激活技术.

- **Date:** 2023-08
- **Pretrain Data Scale:** 2.2T~3T(1.8B:2.2T;7B:2.4T;14B:3.0T)
- **Language Support:** en,zh
- **Parameter Size:** 0.5B/1.8B/4B/7B/14B/72B



### Qwen1.5

[![AI Blog](https://img.shields.io/badge/AI%20Blog-QWen%20AI-orange.svg)](https://qwen.readthedocs.io/en/latest/) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/QwenLM/Qwen1.5) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/Qwen)

Qwen1.5的各个模型在训练上使用了更多的Token，并针对特定任务如代码生成进行了指令微调。例如，CodeQwen1.5专门针对编程任务进行了优化，预训练了大约3万亿个与代码相关的数据Token。

- **Date:** 2023-02
- **Pretrain Data Scale:** 3T
- **Language Support:** en,zh
- **Parameter Size:** 0.5B/1.8B/4B/7B/14B/72B



### Vicuna

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Vicuna%20AI-orange.svg)](https://lmsys.org/blog/2023-03-30-vicuna/) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/lm-sys/FastChat) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/lmsys)

1. **内存优化**：为应对Vicuna在处理长上下文时的需求，其最大上下文长度从Alpaca的512增至2048，这显著提高了对GPU内存的需求。为解决这一问题，研究人员采用了梯度检查点（gradient checkpointing）与FlashAttention技术来减轻内存压力。
2. **多轮对话**：通过调整训练损失以适应多轮对话的需求，训练损失的计算仅基于聊天机器人的输出进行。
3. **通过Spot实例降低成本**：数据集规模增大40倍及序列长度增加4倍，对训练提出了更大的挑战。为降低成本，研究人员通过SkyPilot托管的Spot实例，利用抢占自动恢复和自动区域切换功能，使用成本更低的Spot实例。这种策略将7B模型的训练成本从500美元降至约140美元，13B模型的训练成本从大约1000美元降至300美元。

- **Date:** 2023-03
- **Pretrain Data Scale:** 1.4T
- **Language Support:** en,zh
- **Parameter Size:** 7B/13B/33B



### XGen

[![arXiv](https://img.shields.io/badge/arXiv-2309.03450-b31b1b.svg)](https://arxiv.org/abs/2309.03450) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/salesforce/xGen) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/Salesforce/xgen-7b-4k-base)

XGen-7B模型在支持长达8K令牌的输入，通过使用标准密集注意力进行训练，以及在高达1.5T令牌的情况下进行训练，同时在公共领域的教学数据上进行微调，可作为一种通用模型，适用于标准大小的GPU和移动设备。

- **Date:** 2023-07
- **Pretrain Data Scale:** 1.37T
- **Language Support:** en
- **Parameter Size:** 7B



### Falcon

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Falcon%20AI-orange.svg)](https://huggingface.co/blog/falcon-180b) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/falconry/falcon) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/tiiuae)

大量训练数据来自 [RefinedWeb](https://arxiv.org/abs/2306.01116) —— 一个新的基于 CommonCrawl 的网络数据集。使用了 [**多查询注意力 (multiquery attention)**](https://arxiv.org/abs/1911.02150)。原始多头 (head) 注意力方案每个头都分别有一个查询 (query) 、键 (key) 以及值 (value)，而多查询注意力方案改为在所有头上共享同一个键和值。这个技巧对预训练影响不大，但它极大地 [提高了推理的可扩展性](https://arxiv.org/abs/2211.05102): 事实上， **该技巧大大减少了自回归解码期间 K,V 缓存的内存占用，将其减少了 10-100 倍** (具体数值取决于模型架构的配置)，这大大降低了模型推理的内存开销。而内存开销的减少为解锁新的优化带来了可能，如省下来的内存可以用来存储历史对话，从而使得有状态推理成为可能。

- **Date:** 2023-07
- **Pretrain Data Scale:** 2T
- **Language Support:** en,fr
- **Parameter Size:** 1.3B/7.5B/40B/180B



### Phi

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://www.microsoft.com/en-us/research/blog/phi-2-the-surprising-power-of-small-language-models/) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/microsoft/dstoolkit-phi2-finetune) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/microsoft/phi-2)

**训练数据质量：** 利用“教科书质量”的数据，专注于旨在传授常识推理和常识的合成数据集。培训语料库通过精心挑选的网络数据进行扩充，并根据教育价值和内容质量进行过滤。（Phi-2 leverages “textbook-quality” data, focusing on synthetic datasets designed to impart common sense reasoning and general knowledge. The training corpus is augmented with carefully selected web data, filtered based on educational value and content quality.）

**创新的缩放技术：** 微软在开发 Phi-2 时，采用了从其前代模型 Phi-1.5 到 Phi-2 的知识扩展技术。他们利用了 Phi-1.5 模型中已有的知识和学习成果，将这些知识转移到新模型中，从而加速了新模型训练的收敛速度。简单来说，就是让新模型在学习初期就能站在一个更高的起点上，快速达到高性能。这种知识转移的方法不仅提高了训练效率，还显著提升了模型在各种基准测试中的得分。

**优化的Transformer结构**：Phi-2研究人员引入了自定义优化以最大限度地提高效率。

- **Date:** 2023-12
- **Pretrain Data Scale:** 1.4T
- **Language Support:** en
- **Parameter Size:** 1B/1.5B/2B



### Phi3

[![arXiv](https://img.shields.io/badge/arXiv-2404.14219-b31b1b.svg)](https://arxiv.org/abs/2404.14219) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3)

采用了transformer decoder架构，其默认的上下文长度为**4K token**。团队还通过LongRope技术推出了长上下文版本，将上下文长度扩展到**128K token**。由于体积小巧，phi-3-mini模型可以被量化为**4 bit**，使其内存占用仅约为**1.8GB**。团队通过在配备A16仿生芯片的iPhone 14上部署phi-3-mini进行了测试，该模型能够在完全离线的状态下原生运行，并实现了每秒处理超过12个tokens的速度。

训练数据集也是创新点之一，包括经过严格过滤的网络数据和合成数据，这些数据经过精心筛选和优化，使研究人员能够显著减小模型的大小而不影响性能。

- **Date:** 2024-04
- **Pretrain Data Scale:** 3.3T～4.8T
- **Language Support:** en
- **Parameter Size:** 3.8B/7B/14B



### Gemma

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://storage.googleapis.com/deepmind-media/gemma/gemma-report.pdf) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/google-deepmind/gemma) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/google/gemma-release-65d5efbccdbb8c4202ec078b)

可在各类消费级硬件上运行，无需数据量化处理，拥有高达 8K tokens 的处理能力，在 7B 参数级别Gemma 表现出色，比同参数级别的Llama2性能要好一些。与 Google Cloud 集成，可以通过 Vertex AI 或 Google Kubernetes Engine (GKE) 在 Google Cloud 上部署和训练 Gemma。

- **Date:** 2024-02
- **Pretrain Data Scale:** 2T
- **Language Support:** en
- **Parameter Size:** 2B/7B



### Mamba

[![arXiv](https://img.shields.io/badge/arXiv-2312.00752-b31b1b.svg)](https://arxiv.org/abs/2312.00752) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/state-spaces/mamba) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/state-spaces)
- **Date:** 2023-12
- **Pretrain Data Scale:** 10B
- **Language Support:** en
- **Parameter Size:** 130M/370M/790M/1.4B/2.8B

Mamba 2.8B 是一种基于状态空间模型架构的大型语言模型，在处理信息密集型数据（如语言建模）方面可以和传统的 Transformer 模型竞争。

主要创新点如下

1. **选择性状态空间模型（SSMs）**：Mamba 通过基于输入参数化 SSM 参数引入了选择机制。这使得模型可以根据当前令牌沿序列长度维度选择性地传播或遗忘信息，增强了其聚焦相关信息同时丢弃无关数据的能力。

2. **硬件感知并行算法：** 为了克服选择性状态空间模型（SSMs）带来的计算复杂性，Mamba 采用了一种硬件感知算法，使用扫描而非卷积来计算模型

   > 扫描操作在递归计算中更常见，尤其是在处理需要根据输入动态调整参数的模型时，在 Mamba 模型中，由于引入了选择性机制，使得模型的参数可以根据输入动态变化，这破坏了卷积的使用条件。扫描操作按照序列的顺序，一步步地计算序列的状态，允许每一步的计算都可以基于当前的输入和前一状态动态调整。

3. **长上下文处理**：可以达到100万序列长度，在音频处理和基因组学方面性能良好





### Pythia
[![arXiv](https://img.shields.io/badge/arXiv-2304.01373-b31b1b.svg)](https://arxiv.org/abs/2304.01373) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/EleutherAI/pythia) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/EleutherAI/pythia-scaling-suite-64fb5dfa8c21ebb3db7ad2e1)
- **Date:** 2023-04
- **Pretrain Data Scale:** 10B
- **Language Support:** en
- **Parameter Size:** 130M/370M/790M/1.4B/2.8B


Pythia *Scaling Suite*是为促进可解释性研究而开发的模型集合，is a suite of 16 LLMs all trained on public data seen in the exact same order and ranging in size from 70M to 12B parameters.

> 大型语言模型（LLM）套件，是一系列用于科学研究的语言模型的集合。这些模型在设计和实现时注重一致性和可重现性，目的是让研究者能够深入分析和理解大型语言模型在训练和扩展过程中的表现和变化。

Pythia contains two sets of eight models of sizes 70M, 160M, 410M, 1B, 1.4B, 2.8B, 6.9B, and 12B. For each size, there are two models: one trained on the Pile, and one trained on the Pile after the dataset has been globally deduplicated. All 8 model sizes are trained on the exact same data, in the exact same order. 

> Pile 是一个大型的、开源的英文文本数据集，专为训练大型语言模型而设计。它由 22 个不同的、高质量的子数据集组成，这些子数据集包括了从书籍、学术论文、法律文献、在线问答，到编程代码和电影字幕等多种类型的文本。被广泛用于训练包括自回归变换器在内的大型语言模型，详情：[click here](https://pile.eleuther.ai/)。

Pythia套件是唯一一个满足以下三个关键特性的公开发布的LLM套件：

1. 模型覆盖了多个数量级的模型规模。
2. 所有模型都按照相同的顺序在相同的数据上进行训练。
3. 数据和中间检查点可供公开研究使用。

作者还进行了三个语言建模研究的案例研究

1. **数据偏见如何影响学习行为**：研究表明，通过对语言模型的适当干预，可以发现数据中代词的出现频率会影响模型的学习偏差。研究也提出一种可控的方法来分析和减轻模型的偏差问题。
2. **训练顺序是否影响记忆**：研究者发现，泊松模型能够很好地适配数据，这说明训练顺序对于记忆的影响较小。该模型表明，在训练过程的开始或结束阶段，记忆序列并不会更密集地出现，而是在各个检查点之间，可以观察到大致相同数量的记忆序列分布。
3. **预训练术语频率是否影响整个训练过程中的任务性能**：这种相关性在较大的模型中表现得更为明显。较小的模型即便在训练的后期阶段也很难在这些任务上取得准确的结果，表明这些模型无论训练数据中相关信息的频率如何，都无法成功学习这些任务。





### Mistral
[![arXiv](https://img.shields.io/badge/arXiv-2310.06825-b31b1b.svg)](https://arxiv.org/abs/2310.06825) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/mistralai/mistral-common) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/mistralai)

- **Date:** 2023-09
- **Pretrain Data Scale:** 8T
- **Language Support:** en
- **Parameter Size:** 7B

Mistral 7B 超越了以前最好的 130 亿参数模型（Llama 2）在所有评测基准上的表现，并且在推理、数学和代码生成方面超过了最好的 340 亿参数模型（Llama 1），利用分组查询注意力（Grouped-query Attention, GQA）和滑动窗口注意力（Sliding Window Attention, SWA）。GQA 显著提高了推理速度，减少了解码时的内存需求。SWA 能够更有效地处理更长的序列，从而降低计算成本。

Mistral-7B is a decoder-only Transformer with the following architectural choices:

- Sliding Window Attention - Trained with 8k context length and fixed cache size, with a theoretical attention span of 128K tokens
- GQA (Grouped Query Attention) - allowing faster inference and lower cache size.
- Byte-fallback BPE tokenizer - ensures that characters are never mapped to out of vocabulary tokens.



### YI
[![arXiv](https://img.shields.io/badge/arXiv-2403.04652-b31b1b.svg)](https://arxiv.org/abs/2403.04652) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/01-ai/Yi) 
[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/01-ai/yi-2023-11-663f3f19119ff712e176720f)

- **Date:** 2023-11
- **Pretrain Data Scale:**0. 8T～3T
- **Language Support:** Multiple
- **Parameter Size:** 6B/9B/34B

Yi系列包括6B、9B和34B参数规模的基础模型，每个模型的默认上下文窗口为4K，并在推理时可以扩展到32K。

核心亮点有以下几方面

1. **高质量数据预处理**：Yi系列模型使用了严格的清洗管道来确保高质量的训练数据。这包括使用启发式规则和学习过滤器来去除低质量和不适当的内容，确保数据集的纯净度和相关性。
2. **改进的注意力机制**：Yi模型采用了改进的Grouped-Query Attention（GQA）机制，这大大减少了训练和推理的成本，与传统的多头注意力机制相比具有更高的效率。
3. **多模态支持**：Yi系列还包括多模态模型（Yi-VL），这些模型能够处理文本和图像输入，进行多轮对话和视觉问答。
4. **对中文支持更好**：对标chatGPT4在CMMLU、E-Eval、Gaokao 三个主要的中文指标上Yi-34B表现得很好。

> Grouped-Query Attention (GQA) 机制的原理：传统的多头注意力机制中，每个注意力头都有自己独立的查询（Q）、键（K）和值（V）向量。在GQA中，查询头被分成若干组，每组共享一个键（K）和一个值（V）向量。具体来说，如果一个注意力层有`H`个查询头，这些查询头被分成`G`组（`G < H`），每组共享相同的K和V向量。
>
> 在GQA机制下，键和值向量的计算次数减少，因为同一组内的多个查询头共享相同的K和V。这减少了矩阵乘法的次数，从而降低了计算复杂度。



### YI-1.5
[![arXiv](https://img.shields.io/badge/arXiv-2403.04652-b31b1b.svg)](https://arxiv.org/abs/2403.04652) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/01-ai/Yi-1.5) 
[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/01-ai/yi-15-2024-05-663f3ecab5f815a3eaca7ca8)

- **Date:** 2023-05
- **Pretrain Data Scale:** 3.6T
- **Language Support:** Multiple
- **Parameter Size:** 6B/9B/34B

Yi-1.5模型预训练在5000亿高质量语料库上，并在300万多样化样本上进行了微调。这种大规模的数据训练使得模型在编程、数学、推理和指令遵循任务上的性能更强。包括34B、9B和6B参数模型，每种模型支持的上下文长度分别为4K、16K和32K。

在Yi-1.5系列中特别是9B模型，采用了**后期层的复制方法**以提高模型性能，同时保持高效的训练。与传统的模型扩展方法相比，这种方法能更好地保持性能，减少损失。

最大的 Yi 1.5. 34B 在基准测试中几乎与 Meta Llama 3 70B 相当。

> Yi-34B-200K在“Needle-in-a-Haystack”测试中的表现从89.3%提高到99.8%







### Zephyr
[![arXiv](https://img.shields.io/badge/arXiv-2310.16944-b31b1b.svg)](https://arxiv.org/abs/2310.16944) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/huggingface/alignment-handbook) 
- **Date:** 2023-05
- **Pretrain Data Scale:** According to LLM
- **Language Support:** en
- **Parameter Size:** 7B

Zephyr 系列大语言模型采用了多样的偏好优化技术，使其更符合特定的用户偏好或任务需求。这个系列共有三个模型，每个模型使用了不同的偏好优化算法和底座LLM。

> 偏好优化技术可以确保生成的输出更符合期望，**减少不良输出**，可以极大地增强模型的定制化能力。



#### Zephyr-7B

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/HuggingFaceH4/zephyr-7b-6538c6d6d5ddd1cbb1744a66
)

Zephyr-7B-β 是Zephyr 系列列中的第一个模型，是基于 [Mistralai/Mistral-7B-v0.1](https://link.zhihu.com/?target=https%3A//huggingface.co/mistralai/Mistral-7B-v0.1) 微调而来的，使用的是**直接偏好优化（DPO）**算法

此外该模型利用知识蒸馏技术，即用较小的“学生”模型学习和复制较大“教师”模型的性能。这使得Zephyr-7B在保留较大模型能力的同时，具有更高的计算效率，并且更容易部署在计算资源有限的设备上。

使用的数据集是UltraChat和UltraFeedback数据集

- UltraChat是由ChatGPT生成的合成对话数据集
- UltraFeedback包含了各种提示和响应，并由GPT-4进行了注释

>直接偏好优化（Direct Preference Optimization, DPO）通过直接最大化模型生成的首选响应的概率来进行偏好对齐。DPO算法通过直接优化模型生成的首选响应的概率，而不需要参考模型，简化了训练过程。



#### Zephyr ORPO
[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/HuggingFaceH4/zephyr-orpo-6617eba2c5c0e2cc3c151524)

Zephyr-ORPO-141B-A35b-v0.1是一个具有 141B 总参数和 39B 有效参数的专家混合 （MoE） 模型，是在[Mixtral-8x22B-v0.1](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1)的基础上微调的。采用[Odds Ratio Preference Optimization (ORPO)](https://huggingface.co/papers/2403.07691)算法进行偏好优化，ORPO 不需要 SFT 步骤即可实现高性能，因此计算效率比 DPO 和 PPO 等方法高得多。

ORPO模型通过动态惩罚机制还可以有效地减少了不良响应的生成，确保输出内容的高质量和适用性。

> **Odds Ratio Preference Optimization (ORPO)** 算法通过计算首选响应和非首选响应的赔率比进行优化，确保模型更倾向于生成首选响应。



#### Zephyr-7B Gemma
[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/HuggingFaceH4/zephyr-7b-gemma-65e1fd82d26b426e3e63d956)

是在HuggingFaceH4/deita-10k-v0-sft 数据集上 [google/gemma-7b](https://huggingface.co/google/gemma-7b) 的微调版本，使用的也是DPO的偏好优化算法。



### StripedHyena
[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://www.together.ai/blog/stripedhyena-7b) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/togethercomputer/stripedhyena) 

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/togethercomputer/stripedhyena-65d8e6e77540dd1da932dbe1)

-  2023-12
- **Pretrain Data Scale:** 2T
- **Language Support:** Multiple
- **Parameter Size:** 7B

该模型系列包括 StripedHyena-Hessian-7B 和 StripedHyena-Nous-7B 两个主要变种。[前者](https://huggingface.co/togethercomputer/StripedHyena-Hessian-7B)为基础模型[后者](https://huggingface.co/togethercomputer/StripedHyena-Nous-7B)为聊天模型

StripedHyena 采用了一种混合架构，结合了门控卷积（gated convolutions）和分组查询注意力机制（grouped-query attention）。该模型的核心组件是状态空间模型（SSM）层，传统上用于建模复杂序列和时间序列数据。SSM 层能够更高效地处理长序列任务，减少计算资源需求，相较于经典的 Transformer，在长序列训练中速度更快。

StripedHyena 训练序列长度可达 32k，能够处理更长的提示



### Persimmon
[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://www.adept.ai/blog/persimmon-8b) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/persimmon-ai-labs/adept-inference) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/adept/persimmon-8b-chat)

- **Date:** 2023-09
- **Pretrain Data Scale:**  0.737T
- **Language Support:** en
- **Parameter Size:** 8B

Persimmon-8B 支持 16K 的上下文长度，是 LLaMA2 的四倍，GPT-3 的八倍

采用了一些架构优化，包括平方 ReLU 激活函数和旋转位置编码（rotary positional encodings）。

模型的输入和输出嵌入进行了分离优化，避免了大嵌入层梯度的全量减少，从而提升了训练效率。







## 模型评估平台

### OpenLLM Leaderboard by Hugging Face[[Leaderboard]](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

Hugging Face的OpenLLM排行榜是一个旨在追踪、评级和评估开源大型语言模型（LLMs）和聊天机器人的平台。这个排行榜提供了一个集中的平台。

[Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard) is actually just a wrapper running the open-source benchmarking library [Eleuther AI LM Evaluation Harness](https://github.com/EleutherAI/lm-evaluation-harness) created by the [EleutherAI non-profit AI research lab](https://www.eleuther.ai/) famous for creating [The Pile](https://pile.eleuther.ai/) and training [GPT-J](https://huggingface.co/EleutherAI/gpt-j-6b), [GPT-Neo-X 20B](https://huggingface.co/EleutherAI/gpt-neox-20b), and [Pythia](https://github.com/EleutherAI/pythia). A team with serious credentials in the AI space!（Citation from Hugging Face blog）



### Chatbot Arena by LMSYS and SkyLab[[Chatbot Arena]](https://arena.lmsys.org/)

Chatbot Arena的主要功能介绍：

1. **模型对战（Arena Battle）**：在Chatbot Arena中，用户可以选择两个不同的匿名模型（如ChatGPT、Claude、Llama等），并将它们进行对比。在一个安全的比赛环境中，用户可以提问并评估两个模型的回答，通过投票决定哪个模型表现更出色。这一比较过程可以多轮进行，直到确定最终的胜利者。为了保证比赛的公平性，如果某轮对话暴露了模型的具体身份，该轮的投票结果将被排除。
2. **实时聊天（Direct Chat）**：Chatbot Arena提供了一个实时聊天功能，允许用户直接与选定的模型进行对话。无论用户选择的是文本还是视觉聊天模式，都能即时接收到模型的反馈。
3. **排行榜（Leaderboard）**：Chatbot Arena通过分析超过300,000个人类用户的投票结果，采用基于Elo系统的方法来评估各个LLM的排名。这让用户能够直观地了解哪些模型当前处于领先地位，轻松识别出LLM领域的佼佼者。



## 基准测试

### ARC (AI2 Reasoning Challenge)

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-arc%20challenge-blue.svg)](https://paperswithcode.com/sota/common-sense-reasoning-on-arc-challenge)
[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-arc%20easy-blue.svg)](https://paperswithcode.com/sota/common-sense-reasoning-on-arc-easy)
[![arXiv](https://img.shields.io/badge/arXiv-2305.18354-b31b1b.svg)](https://arxiv.org/pdf/2305.18354) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/fchollet/ARC) 

ARC（Abstraction and Reasoning Corpus）基准是一个用于评估大型语言模型性能的挑战性框架，特别是在执行需要抽象和推理任务的能力方面。这个基准测试是推动AI模型超越当前许多基准中常见的标准模式识别任务的一部分。

##### ARC的主要特点

- **任务设计**：ARC中的任务设计对人类来说很简单，但对AI来说却很有挑战性。每个任务包括一个输入和一个正确的输出，目标是通过辨别底层模式或规则，从输入中预测输出。任务涵盖各种认知功能，包括模式识别、空间推理和逻辑推理。
- **数据集**：ARC数据集是公开的，包括训练集和测试集，其中测试集包含完全新颖的任务，需要超越训练数据进行泛化。这种设置旨在模拟现实世界的学习场景，在这些场景中并非总能直接获得答案，必须应用推理。
- **评估**：在ARC中取得成功需要开发能够真正理解和操作抽象概念的模型，这使其成为测试AI推理能力的严格标准，而不仅仅是其数据处理能力的测试。



### HellaSwag

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-hellaswag-blue.svg)](https://paperswithcode.com/sota/sentence-completion-on-hellaswag)
[![arXiv](https://img.shields.io/badge/arXiv-1905.07830-b31b1b.svg)](https://arxiv.org/abs/1905.07830) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/rowanz/hellaswag) 

**HellaSwag**是一个用于评估语言模型在常识自然语言推理方面表现的基准。它特别测试模型预测日常活动简单描述的延续部分的能力，这些描述对人类来说显而易见，但对算法来说可能具有挑战性。该基准包含大量选择题，每题提供一个场景和四个可能的延续，模型必须从中选择最合适的一个。

HellaSwag中的问题主要来自两个领域：ActivityNet和WikiHow，丰富了数据集的实际相关性和多样性。正确答案描述了实际的下一个事件，而其他三个错误选项是对抗性生成并经人工验证，旨在误导模型但不误导人类。

HellaSwag的构建包括一种“对抗性过滤”技术，一系列判别器反复选择机器生成的错误答案，这些答案能够有效地欺骗模型。这种方法在挑战模型识别现实场景方面已被证明有效，并且突出了即使是最先进模型的局限性。



### MMLU (Massive Multitask Language Understanding)

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-MMLU-blue.svg)](https://paperswithcode.com/sota/multi-task-language-understanding-on-mmlu?tag_filter=183)
[![arXiv](https://img.shields.io/badge/arXiv-2009.03300-b31b1b.svg)](https://arxiv.org/abs/2009.03300) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/hendrycks/test) 

这是一个广泛而多样的基准，用于评估模型在从人文学科到科学等广泛主题上的理解能力。它旨在测试模型在各种主题上的一般知识和理解能力。

> 注意：MMLU的评估包含三种形式，分别是MMLU (HELM)、MMLU (Harness)和MMLU (Original)。曾经，在Hugging Face的OpenLLM排行榜上，[**LLaMA model 🦙**](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/)被爆出MMLU评估结果明显低于[已发表的 LLaMa 论文](https://arxiv.org/abs/2302.13971)中的数字。最终[Blog](https://huggingface.co/blog/open-llm-leaderboard-mmlu)上的声明将这个现象归结为用于测试的MMLU benchmark的细节不同导致了结果不同，详情可参见[Blog](https://huggingface.co/blog/open-llm-leaderboard-mmlu)



### TruthfulQA

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-truthfulqa-blue.svg)](https://paperswithcode.com/sota/question-answering-on-truthfulqa)
[![arXiv](https://img.shields.io/badge/arXiv-2109.07958-b31b1b.svg)](https://arxiv.org/abs/2109.07958) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/sylinrl/TruthfulQA) 

该基准评估模型提供真实答案的能力。它通过测试模型如何处理可能通常会导致不真实或误导性答案的问题来减少错误信息的传播。

**TruthfulQA**是一个评估大型语言模型生成真实答案能力的基准。它包含38个类别中的817个问题，包括健康、法律、金融和政治等领域。问题旨在考察模型处理人类可能因误解或错误信念而回答错误的场景的能力。TruthfulQA的主要目标是衡量模型生成真实响应的准确性。基准使用各种任务和模式，包括单选和多选题以及生成任务，以评估模型识别和生成真实答案的能力。

##### 任务和评估方法

TruthfulQA包括两个主要任务：

1. **生成任务**：模型接收一个问题并生成一到两句话的答案。此任务的主要指标是模型答案的整体真实性，评估标准是描述现实世界中的字面真实情况。次要指标包括信息量，通过评估模型提供有意义的信息而不是模棱两可的响应。
2. **多选任务**：此任务有两种形式：
   - **MC1（单一真实）**：模型接收一个问题和若干答案选项，必须选择唯一正确的答案。
   - **MC2（多重真实）**：模型接收多个真实和虚假的参考答案，必须识别所有正确答案。

##### 重要点

- **对抗性**：TruthfulQA中的问题是对抗性设计的，测试模型生成真实答案的潜在弱点。这包括设计利用常见误解的问题，或者由于模型训练数据的偏差可能会错误回答的问题。
- **验证和基准**：该基准包括验证机制，外部研究人员评估参考答案的真实性和准确性，确保基准评估的稳健性。



### Winogrande

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-Winogrande-blue.svg)](https://paperswithcode.com/sota/common-sense-reasoning-on-winogrande)
[![arXiv](https://img.shields.io/badge/arXiv-1907.10641-b31b1b.svg)](https://arxiv.org/pdf/1907.10641) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/allenai/winogrande) 

WINOGRANDE是一个基于Winograd Schema Challenge（WSC）的语言理解基准，旨在评估大型语言模型在解决需要常识和推理能力的代词解析问题上的表现。通过提供比原始WSC更大和更具挑战性的数据集，WINOGRANDE更适合评估现代人工智能语言模型的能力。

由艾伦人工智能研究所开发，WINOGRANDE基准的目的是通过代词解析任务测试模型的推理能力。这些任务通常涉及一个带有代词和多个潜在指代的句子，模型需要确定代词的正确指代。例如：

```less
Sentence: The elephant put the apple there because it was ______.
Options: A) empty B) heavy
Correct Answer: A) empty

Sentence: The trophy doesn’t fit into the suitcase because it is too small.“It” refers ______.
Options: A) the trophy B) the suitcase
Correct Answer: B) the suitcase
```

这种类型的问题要求模型不仅理解语言的字面意思，还需要推理出上下文中的隐含关系。	

### GSM8K (Grade School Math 8K)

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-GSM8K-blue.svg)](https://paperswithcode.com/dataset/gsm8k)
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/openai/grade-school-math) 

GSM8K（Grade School Math 8K）数据集由OpenAI开发，旨在评估大型语言模型解决小学水平数学问题的能力。该基准包含8500个高质量、语言多样的数学文字问题，需要进行基本的算术运算如加法、减法、乘法和除法。这些问题通常需要两到八步解决。数据集分为7500个训练问题和1000个测试问题，旨在测试模型在多步骤数学推理中的能力。GSM8K对于评估模型处理涉及顺序逻辑和计算步骤的问题非常有用。

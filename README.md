# awesome-list-of-LLM_VLMs
github awesome list of recent LLMs and VLMs.

Here is list of LLMs, to reach list of VLMs. Click [here]()

## Quick Start

|  Model  | Parameters              | CheckPoint                                                   |
| :-----: | ----------------------- | ------------------------------------------------------------ |
| Llama 2 | 7B/13B/70B              | [Llama2 Family](https://huggingface.co/collections/meta-llama/llama-2-family-661da1f90a9d678b6f55773b) |
| Llama 3 | 8B/70B                  | [Llama3 Family](https://huggingface.co/collections/meta-llama/meta-llama-3-66214712577ca38149ebb2b6) |
|  Qwen   | 0.5B/1.8B/4B/7B/14B/72B | [Qwen](https://huggingface.co/Qwen)                          |
| Qwen1.5 | 0.5B/1.8B/4B/7B/14B/72B | [Qwen1.5](https://huggingface.co/Qwen)                       |
| Vicuna  | 7B/13B/33B              | [Vicuna](https://huggingface.co/lmsys)                       |
|  XGen   | 7B                      | [xgen-7b-4k-base](https://huggingface.co/Salesforce/xgen-7b-4k-base) |
| Falcon  | 1.3B/7.5B/40B/180B      | [Falcon Family](https://huggingface.co/collections/tiiuae/falcon-64fb432660017eeec9837b5a) |
|   phi   | 1B/1.5B/2B              | [phi-1B()](https://huggingface.co/microsoft/phi-1)<br />[phi-1.5B](https://huggingface.co/microsoft/phi-1_5)<br />[phi-2B](https://huggingface.co/microsoft/phi-2) |
|  phi3   | 3.8B/7B/14B             | [Phi-3 family**(only phi-3-mini is available now)**](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3) |
|  Gemma  | 2B/7B                   | [GemmaFamily](https://huggingface.co/collections/google/gemma-release-65d5efbccdbb8c4202ec078b) |



## Details Regarding Models Above

### Llama 2



Llama 2预训练模型相较于 Llama 1 模型有显著提升，增加了 40% 的训练词元总数，并采用了更长的上下文长度（高达 4000 词元），同时还利用分组查询注意力机制，极大加速了 70B 模型的推理速度。Llama 2-Chat 系列模型采用了基于人类反馈的强化学习（RLHF）技术，专门针对对话场景进行优化。在广泛的有用性和安全性测试基准中，Llama 2-Chat 的表现超过了多数现有开放模型，并且在人类评估中显示出与 ChatGPT 相媲美的性能。

- **Date:** 2023-07
- **Pretrain Data Scale:**2T
- **Language Support:**en
- **Parameter Size:**7B/13B/70B



### Llama 3



相较于 Llama 2，Llama 3 最显著的变化在于引入了一个新的 Tokenizer，并将词汇表的规模扩展到了 128,256 个词汇（先前版本为 32,000 个 Token）。这样一个更庞大的词汇表可以更有效地对文本进行编码，无论是输入还是输出，也可能增强模型处理多语言的能力。然而，这一改变同时导致了嵌入层的输入和输出矩阵的尺寸增大，从而增加了小型模型的参数量。

- **Date:** 2024-04
- **Pretrain Data Scale:**1.5T
- **Language Support:**en
- **Parameter Size:**8B/70B



### Qwen



通过指令微调（Instruction Fine-Tuning）对特定任务进行优化，比如编程语言生成（CodeQwen），采用了混合专家（Mixture of Experts, MoE）和稀疏激活技术.

- **Date:** 2023-08
- **Pretrain Data Scale:**2.2T~3T(1.8B:2.2T;7B:2.4T;14B:3.0T)
- **Language Support:**en,zh
- **Parameter Size:**0.5B/1.8B/4B/7B/14B/72B



### Qwen1.5



Qwen1.5的各个模型在训练上使用了更多的Token，并针对特定任务如代码生成进行了指令微调。例如，CodeQwen1.5专门针对编程任务进行了优化，预训练了大约3万亿个与代码相关的数据Token。

- **Date:** 2023-02
- **Pretrain Data Scale:**3T
- **Language Support:**en,zh
- **Parameter Size:**0.5B/1.8B/4B/7B/14B/72B



### Vicuna



1. **内存优化**：为应对Vicuna在处理长上下文时的需求，其最大上下文长度从Alpaca的512增至2048，这显著提高了对GPU内存的需求。为解决这一问题，研究人员采用了梯度检查点（gradient checkpointing）与FlashAttention技术来减轻内存压力。
2. **多轮对话**：通过调整训练损失以适应多轮对话的需求，训练损失的计算仅基于聊天机器人的输出进行。
3. **通过Spot实例降低成本**：数据集规模增大40倍及序列长度增加4倍，对训练提出了更大的挑战。为降低成本，研究人员通过SkyPilot托管的Spot实例，利用抢占自动恢复和自动区域切换功能，使用成本更低的Spot实例。这种策略将7B模型的训练成本从500美元降至约140美元，13B模型的训练成本从大约1000美元降至300美元。

- **Date:** 2023-03
- **Pretrain Data Scale:**1.4T
- **Language Support:**en,zh
- **Parameter Size:**7B/13B/33B



### XGen



XGen-7B模型在支持长达8K令牌的输入，通过使用标准密集注意力进行训练，以及在高达1.5T令牌的情况下进行训练，同时在公共领域的教学数据上进行微调，可作为一种通用模型，适用于标准大小的GPU和移动设备。

- **Date:** 2023-07
- **Pretrain Data Scale:**1.37T
- **Language Support:**en
- **Parameter Size:**7B



### Falcon



大量训练数据来自 [RefinedWeb](https://arxiv.org/abs/2306.01116) —— 一个新的基于 CommonCrawl 的网络数据集。使用了 [**多查询注意力 (multiquery attention)**](https://arxiv.org/abs/1911.02150)。原始多头 (head) 注意力方案每个头都分别有一个查询 (query) 、键 (key) 以及值 (value)，而多查询注意力方案改为在所有头上共享同一个键和值。这个技巧对预训练影响不大，但它极大地 [提高了推理的可扩展性](https://arxiv.org/abs/2211.05102): 事实上， **该技巧大大减少了自回归解码期间 K,V 缓存的内存占用，将其减少了 10-100 倍** (具体数值取决于模型架构的配置)，这大大降低了模型推理的内存开销。而内存开销的减少为解锁新的优化带来了可能，如省下来的内存可以用来存储历史对话，从而使得有状态推理成为可能。

- **Date:** 2023-07
- **Pretrain Data Scale:**2T
- **Language Support:**en,fr
- **Parameter Size:**1.3B/7.5B/40B/180B



### phi

**训练数据质量：**利用“教科书质量”的数据，专注于旨在传授常识推理和常识的合成数据集。培训语料库通过精心挑选的网络数据进行扩充，并根据教育价值和内容质量进行过滤。（Phi-2 leverages “textbook-quality” data, focusing on synthetic datasets designed to impart common sense reasoning and general knowledge. The training corpus is augmented with carefully selected web data, filtered based on educational value and content quality.）

**创新的缩放技术：**微软在开发 Phi-2 时，采用了从其前代模型 Phi-1.5 到 Phi-2 的知识扩展技术。他们利用了 Phi-1.5 模型中已有的知识和学习成果，将这些知识转移到新模型中，从而加速了新模型训练的收敛速度。简单来说，就是让新模型在学习初期就能站在一个更高的起点上，快速达到高性能。这种知识转移的方法不仅提高了训练效率，还显著提升了模型在各种基准测试中的得分。

**优化的Transformer结构**：Phi-2研究人员引入了自定义优化以最大限度地提高效率。

- **Date:** 2023-12
- **Pretrain Data Scale:**1.4T
- **Language Support:**en
- **Parameter Size:**1B/1.5B/2B



### phi3



采用了transformer decoder架构，其默认的上下文长度为**4K token**。团队还通过LongRope技术推出了长上下文版本，将上下文长度扩展到**128K token**。由于体积小巧，phi-3-mini模型可以被量化为**4 bit**，使其内存占用仅约为**1.8GB**。团队通过在配备A16仿生芯片的iPhone 14上部署phi-3-mini进行了测试，该模型能够在完全离线的状态下原生运行，并实现了每秒处理超过12个tokens的速度。

训练数据集也是创新点之一，包括经过严格过滤的网络数据和合成数据，这些数据经过精心筛选和优化，使研究人员能够显著减小模型的大小而不影响性能。

- **Date:** 2024-04
- **Pretrain Data Scale:**3.3T～4.8T
- **Language Support:**en
- **Parameter Size:**3.8B/7B/14B







## 模型评估汇总

Hugging face中的实时排行榜：[Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

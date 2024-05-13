# awesome-list-of-LLM_VLMs🌐✨
github awesome list of recent LLMs and VLMs.

Here is list of **LLMs**, to reach list of VLMs. Click [here](https://github.com/HuBocheng/awesome-list-of-LLM_VLMs/blob/master/README_VLMs.md)🚀



## Quick Start🏁

|  Model  | Organization |       Parameters        |                          CheckPoint                          |      Details       |
| :-----: | :----------: | :---------------------: | :----------------------------------------------------------: | :----------------: |
| Llama 2 |     Meta     |       7B/13B/70B        | [Llama2 Family](https://huggingface.co/collections/meta-llama/llama-2-family-661da1f90a9d678b6f55773b) | [Llama2](#llama2)  |
| Llama 3 |     Meta     |         8B/70B          | [Llama3 Family](https://huggingface.co/collections/meta-llama/meta-llama-3-66214712577ca38149ebb2b6) | [Llama3](#llama3)  |
|  Qwen   |   Alibaba    | 0.5B/1.8B/4B/7B/14B/72B |             [Qwen](https://huggingface.co/Qwen)              |   [Qwen](#qwen)    |
| Qwen1.5 |   Alibaba    | 0.5B/1.8B/4B/7B/14B/72B |            [Qwen1.5](https://huggingface.co/Qwen)            | [Qwen1.5](#qwen15) |
| Vicuna  |    LMSYS     |       7B/13B/33B        |            [Vicuna](https://huggingface.co/lmsys)            | [Vicuna](#vicuna)  |
|  XGen   |  Salesforce  |           7B            | [xgen-7b-4k-base](https://huggingface.co/Salesforce/xgen-7b-4k-base) |   [XGen](#xgen)    |
| Falcon  |     UAE      |   1.3B/7.5B/40B/180B    | [Falcon Family](https://huggingface.co/collections/tiiuae/falcon-64fb432660017eeec9837b5a) | [Falcon](#falcon)  |
|   phi   |  Microsoft   |       1B/1.5B/2B        | [phi-1B()](https://huggingface.co/microsoft/phi-1)<br />[phi-1.5B](https://huggingface.co/microsoft/phi-1_5)<br />[phi-2B](https://huggingface.co/microsoft/phi-2) |    [phi](#phi)     |
|  phi3   |  Microsoft   |       3.8B/7B/14B       | [Phi-3 family **(only phi-3-mini is available now)**](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3) |   [phi3](#phi3)    |
|  Gemma  |    Google    |          2B/7B          | [GemmaFamily](https://huggingface.co/collections/google/gemma-release-65d5efbccdbb8c4202ec078b) |  [Gemma](#gemma)   |



## Details Regarding Models Above📊

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



## 模型评估平台

### OpenLLM Leaderboard by Hugging Face[[Leaderboard]](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

Hugging Face的OpenLLM排行榜是一个旨在追踪、评级和评估开源大型语言模型（LLMs）和聊天机器人的平台。这个排行榜提供了一个集中的平台。

[Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard) is actually just a wrapper running the open-source benchmarking library [Eleuther AI LM Evaluation Harness](https://github.com/EleutherAI/lm-evaluation-harness) created by the [EleutherAI non-profit AI research lab](https://www.eleuther.ai/) famous for creating [The Pile](https://pile.eleuther.ai/) and training [GPT-J](https://huggingface.co/EleutherAI/gpt-j-6b), [GPT-Neo-X 20B](https://huggingface.co/EleutherAI/gpt-neox-20b), and [Pythia](https://github.com/EleutherAI/pythia). A team with serious credentials in the AI space!（Citation from Hugging Face blog）



### Chatbot Arena by LMSYS and SkyLab[[Chatbot Arena]](https://arena.lmsys.org/)

Chatbot Arena的主要功能介绍：

1. **模型对战（Arena Battle）**：在Chatbot Arena中，用户可以选择两个不同的匿名模型（如ChatGPT、Claude、Llama等），并将它们进行对比。在一个安全的比赛环境中，用户可以提问并评估两个模型的回答，通过投票决定哪个模型表现更出色。这一比较过程可以多轮进行，直到确定最终的胜利者。为了保证比赛的公平性，如果某轮对话暴露了模型的具体身份，该轮的投票结果将被排除。
2. **实时聊天（Direct Chat）**：Chatbot Arena提供了一个实时聊天功能，允许用户直接与选定的模型进行对话。无论用户选择的是文本还是视觉聊天模式，都能即时接收到模型的反馈。
3. **排行榜（Leaderboard）**：Chatbot Arena通过分析超过300,000个人类用户的投票结果，采用基于Elo系统的方法来评估各个LLM的排名。这让用户能够直观地了解哪些模型当前处于领先地位，轻松识别出LLM领域的佼佼者。



## Benchmarks

### ARC (AI2 Reasoning Challenge)

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-arc%20challenge-blue.svg)](https://paperswithcode.com/sota/common-sense-reasoning-on-arc-challenge)
[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-arc%20easy-blue.svg)](https://paperswithcode.com/sota/common-sense-reasoning-on-arc-easy)
[![arXiv](https://img.shields.io/badge/arXiv-2305.18354-b31b1b.svg)](https://arxiv.org/pdf/2305.18354) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/fchollet/ARC) 

The ARC (Abstraction and Reasoning Corpus) benchmark is a challenging framework used to evaluate the performance of large language models, particularly in their ability to perform tasks that require both abstraction and reasoning. This benchmark is part of an effort to push the boundaries of what AI models can achieve beyond standard pattern recognition tasks that are common in many benchmarks today.

##### Key Features of ARC

- **Task Design**: The tasks in ARC are designed to be straightforward for humans but challenging for AI. Each task involves an input and a correct output, with the goal being to predict the output from the input by discerning the underlying pattern or rule. The tasks cover various types of cognitive functions, including pattern recognition, spatial reasoning, and logical deduction.
- **Dataset**: The ARC dataset is publicly available and consists of a training set and a test set, where the test set contains completely novel tasks that require generalizing beyond the training data. This setup is intended to simulate real-world learning scenarios where direct answers are not always available, and reasoning must be applied.
- **Evaluation**: Success in ARC requires developing models that can truly understand and manipulate abstract concepts, making it a stringent test of an AI’s reasoning abilities rather than just its data processing capabilities.



### HellaSwag

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-hellaswag-blue.svg)](https://paperswithcode.com/sota/sentence-completion-on-hellaswag)
[![arXiv](https://img.shields.io/badge/arXiv-1905.07830-b31b1b.svg)](https://arxiv.org/abs/1905.07830) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/rowanz/hellaswag) 

**HellaSwag** is a benchmark designed to evaluate the performance of language models on commonsense natural language inference. It specifically tests the model's ability to predict the continuation of straightforward descriptions of everyday activities, which are obvious to humans but potentially challenging for algorithms. The benchmark consists of numerous multiple-choice questions, each providing a scenario and four possible continuations, from which the model must select the most appropriate one.

The questions in HellaSwag primarily derive from two domains: ActivityNet and WikiHow, enriching the dataset with practical relevance and diversity. The correct answer describes the actual next event, while the other three incorrect options are adversarially generated and human-verified to mislead models but not humans.

The construction of HellaSwag includes an "Adversarial Filtering" technique, where a series of discriminators iteratively select machine-generated wrong answers that effectively deceive models. This method has proven its effectiveness in challenging models to recognize real-world scenarios and has highlighted the limitations of even state-of-the-art models.



### MMLU (Massive Multitask Language Understanding)

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-MMLU-blue.svg)](https://paperswithcode.com/sota/multi-task-language-understanding-on-mmlu?tag_filter=183)
[![arXiv](https://img.shields.io/badge/arXiv-2009.03300-b31b1b.svg)](https://arxiv.org/abs/2009.03300) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/hendrycks/test) 

This is a broad and diverse benchmark that evaluates a model's understanding across a wide range of subjects, from humanities to science. It's designed to test the model's general knowledge and understanding capabilities on various topics.

> 注意：MMLU的评估包含三种形式，分别是MMLU (HELM)、MMLU (Harness)和MMLU (Original)。曾经，在Hugging Face的OpenLLM排行榜上，[**LLaMA model 🦙**](https://ai.facebook.com/blog/large-language-model-llama-meta-ai/)被爆出MMLU评估结果明显低于[已发表的 LLaMa 论文](https://arxiv.org/abs/2302.13971)中的数字。最终[Blog](https://huggingface.co/blog/open-llm-leaderboard-mmlu)上的声明将这个现象归结为用于测试的MMLU benchmark的细节不同导致了结果不同，详情可参见[Blog](https://huggingface.co/blog/open-llm-leaderboard-mmlu)



### TruthfulQA

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-truthfulqa-blue.svg)](https://paperswithcode.com/sota/question-answering-on-truthfulqa)
[![arXiv](https://img.shields.io/badge/arXiv-2109.07958-b31b1b.svg)](https://arxiv.org/abs/2109.07958) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/sylinrl/TruthfulQA) 

This benchmark evaluates a model's ability to provide truthful answers. It focuses on minimizing the spread of misinformation by testing how models handle questions that might typically lead to untruthful or misleading answers.

**TruthfulQA** is a benchmark designed to assess the truthfulness of answers generated by large language models. It consists of 817 questions across 38 categories, including sectors like health, law, finance, and politics. The questions are designed to probe models on their ability to handle scenarios where humans might respond incorrectly due to misconceptions or false beliefs. The main goal of TruthfulQA is to measure how accurately models can generate truthful responses. The benchmark employs various tasks and modes, including single and multiple-choice questions as well as generative tasks, to evaluate a model's capacity to identify and generate truthful answers.

##### Tasks and Evaluation Methods

TruthfulQA includes two primary tasks:

1. **Generation Task**: Models are given a question and must generate a one to two-sentence answer. The primary metric for this task is the overall truthfulness of the model’s answers, assessed against a standard where the truth must describe the literal truth about the real world. Secondary metrics include informativeness, assessed by whether the model provides meaningful information rather than evasive responses.
2. **Multiple-Choice Task**: This task comes in two forms:
   - **MC1 (Single-true)**: Models are provided with a question and several answer choices, and they must select the single correct answer.
   - **MC2 (Multi-true)**: Models are given multiple true and false reference answers and must identify all correct answers.

##### Important Points

- **Adversarial Nature**: The questions in TruthfulQA are adversarially designed to test models on potential weaknesses in generating truthful answers. This includes crafting questions that leverage common misconceptions or that models might commonly answer falsely due to their training on biased data distributions.
- **Validation and Benchmarks**: The benchmark includes validation mechanisms where external researchers assess the truthfulness and accuracy of the reference answers, ensuring the robustness of the benchmark's evaluations.



### Winogrande

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-Winogrande-blue.svg)](https://paperswithcode.com/sota/common-sense-reasoning-on-winogrande)
[![arXiv](https://img.shields.io/badge/arXiv-1907.10641-b31b1b.svg)](https://arxiv.org/pdf/1907.10641) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/allenai/winogrande) 

WINOGRANDE is a language understanding benchmark based on the Winograd Schema Challenge (WSC) designed to evaluate the performance of large language models (LLMs) in solving pronoun resolution problems that require common sense and reasoning abilities. By offering a larger and more challenging dataset than the original WSC, WINOGRANDE is better suited for assessing the capabilities of modern artificial intelligence language models.

Developed by the Allen Institute for AI, the purpose of the WINOGRANDE benchmark is to test models' reasoning abilities through pronoun resolution tasks. These tasks typically involve a sentence with a pronoun and multiple potential referents, and the model needs to determine the correct referent for the pronoun. For example:

```less
Sentence: The elephant put the apple there because it was ______.
Options: A) empty B) heavy
Correct Answer: A) empty
```

This type of question requires the model to understand not just the literal meaning of the language but also to reason about implicit relationships within the context.



### GSM8K (Grade School Math 8K)

[![Paper with Code](https://img.shields.io/badge/Paper%20with%20Code-GSM8K-blue.svg)](https://paperswithcode.com/dataset/gsm8k)
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/openai/grade-school-math) 

The GSM8K (Grade School Math 8K) dataset, developed by OpenAI, is designed to evaluate the performance of large language models on solving elementary school-level math problems. The benchmark consists of 8,500 high-quality, linguistically diverse math word problems that require basic arithmetic operations such as addition, subtraction, multiplication, and division. These problems typically take between two to eight steps to solve. The dataset is divided into 7,500 training problems and 1,000 test problems, aimed at testing the models' capabilities in multi-step mathematical reasoning. GSM8K is particularly useful for assessing how well models handle problems that involve sequential logic and computational steps.



## Quantitative metrics for large model inference

Quantitative metrics for large model inference using NVIDIA GPUs and Apple Silicon chips, please reach [here](https://github.com/XiongjieDai/GPU-Benchmarks-on-LLM-Inference)


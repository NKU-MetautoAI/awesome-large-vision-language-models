<div align="center">
  <img src="./image/title.png" width="800" />
</div>
<div align="center">
<strong>🌐✨github awesome list of recent 🔥LLMs🔥</strong><br>
<strong><a href="./README_LLM_zh.md">中文🚀</a></strong> | <strong>English</strong><br>
<strong>LLMs</strong> | <strong><a href="./README_LVLMs.md">VLMs🚀</a></strong>
</div>

## OverView

<div align="center">
  <img src="./image/LLM2023.png"  width="800" />
</div>
<div align="center">
  <img src="./image/LLM2024.png"  width="800" />
</div>
*<em>Image source: <a href="https://lifearchitect.ai/models">LifeArchitect.ai/models</a></em>*

## Details Regarding Models Above📊

### YI-1.5

[![arXiv](https://img.shields.io/badge/arXiv-2403.04652-b31b1b.svg)](https://arxiv.org/abs/2403.04652) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/01-ai/Yi-1.5) 
[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/01-ai/yi-15-2024-05-663f3ecab5f815a3eaca7ca8)

- **Date:** 2024-05
- **Pretrain Data Scale:** 3.6T
- **Language Support:** Multiple
- **Parameter Size:** 6B/9B/34B

The Yi-1.5 model is pretrained on a 500 billion high-quality corpus and fine-tuned on 3 million diverse samples. This large-scale data training enhances the model's performance in tasks such as programming, mathematics, reasoning, and instruction following. The series includes models with 34B, 9B, and 6B parameters, supporting context lengths of 4K, 16K, and 32K, respectively.

In the Yi-1.5 series, particularly the 9B model, a **late layer duplication method** is employed to improve model performance while maintaining efficient training. Compared to traditional model scaling methods, this approach better preserves performance and reduces loss.

The largest Yi 1.5, with 34B parameters, performs almost on par with Meta Llama 3 70B in benchmarks.

> Yi-34B-200K's performance in the "Needle-in-a-Haystack" test improved from 89.3% to 99.8%.





### Llama3

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Meta%20AI-orange.svg)](https://ai.meta.com/blog/)
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/meta-llama/llama3)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/meta-llama/meta-llama-3-66214712577ca38149ebb2b6)

Compared to Llama 2, the most notable change in Llama 3 is the introduction of a new tokenizer and an expanded vocabulary size of 128,256 tokens (previously 32,000 tokens). This larger vocabulary allows for more efficient text encoding for both input and output, potentially enhancing the model's multilingual capabilities. However, this change also increases the size of the input and output matrices in the embedding layer, resulting in a larger parameter count for smaller models.

- **Date:** 2024-04
- **Pretrain Data Scale:** 1.5T
- **Language Support:** en
- **Parameter Size:** 8B/70B





### Phi3

[![arXiv](https://img.shields.io/badge/arXiv-2404.14219-b31b1b.svg)](https://arxiv.org/abs/2404.14219) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/microsoft/phi-3-6626e15e9585a200d2d761e3)

The model adopts a transformer decoder architecture with a default context length of **4K tokens**. The team also introduced a long-context version using LongRope technology, extending the context length to **128K tokens**. Due to its compact size, the phi-3-mini model can be quantized to **4 bits**, reducing its memory footprint to approximately **1.8GB**. The team tested the phi-3-mini model on an iPhone 14 equipped with an A16 Bionic chip, where it was able to run natively and completely offline, processing over 12 tokens per second.

The training dataset is also an innovation, comprising strictly filtered web data and synthetic data. These data are carefully selected and optimized, allowing researchers to significantly reduce the model's size without compromising performance.

- **Date:** 2024-04
- **Pretrain Data Scale:** 3.3T～4.8T
- **Language Support:** en
- **Parameter Size:** 3.8B/7B/14B



### Gemma

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://storage.googleapis.com/deepmind-media/gemma/gemma-report.pdf) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/google-deepmind/gemma) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/google/gemma-release-65d5efbccdbb8c4202ec078b)

Gemma can run on various consumer-grade hardware without requiring data quantization, supporting up to 8K tokens. At the 7B parameter level, Gemma performs excellently, outperforming Llama2 at the same parameter level. It integrates with Google Cloud and can be deployed and trained on Google Cloud via Vertex AI or Google Kubernetes Engine (GKE).

- **Date:** 2024-02
- **Pretrain Data Scale:** 2T
- **Language Support:** en
- **Parameter Size:** 2B/7B



### Qwen1.5

[![AI Blog](https://img.shields.io/badge/AI%20Blog-QWen%20AI-orange.svg)](https://qwen.readthedocs.io/en/latest/) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/QwenLM/Qwen1.5) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/Qwen)

The various models of Qwen1.5 were trained using a larger number of tokens and fine-tuned with instructions for specific tasks such as code generation. For example, CodeQwen1.5 is specifically optimized for programming tasks, pre-trained with approximately 3 trillion code-related data tokens.

- **Date:** 2023-02
- **Pretrain Data Scale:** 3T
- **Language Support:** en,zh
- **Parameter Size:** 0.5B/1.8B/4B/7B/14B/72B



### Phi

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://www.microsoft.com/en-us/research/blog/phi-2-the-surprising-power-of-small-language-models/) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/microsoft/dstoolkit-phi2-finetune) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/microsoft/phi-2)

**Training Data Quality:** By leveraging "textbook-quality" data, the focus is on synthetic datasets designed to impart common sense reasoning and general knowledge. The training corpus is augmented with carefully selected web data, filtered based on educational value and content quality.

**Innovative Scaling Techniques:** Microsoft employed knowledge expansion techniques from its predecessor model, Phi-1.5, to Phi-2 during the development of Phi-2. They utilized the existing knowledge and learning outcomes from the Phi-1.5 model, transferring this knowledge to the new model to accelerate its convergence during training. Simply put, this approach allows the new model to start from a higher baseline, achieving high performance quickly. This knowledge transfer method not only enhances training efficiency but also significantly improves the model's scores across various benchmarks.

**Optimized Transformer Architecture:** Phi-2 researchers introduced custom optimizations to maximize efficiency.

- **Date:** 2023-12
- **Pretrain Data Scale:** 1.4T
- **Language Support:** en
- **Parameter Size:** 1B/1.5B/2B



### Mamba

[![arXiv](https://img.shields.io/badge/arXiv-2312.00752-b31b1b.svg)](https://arxiv.org/abs/2312.00752) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/state-spaces/mamba) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/state-spaces)

- **Date:** 2023-12
- **Pretrain Data Scale:** 10B
- **Language Support:** en
- **Parameter Size:** 130M/370M/790M/1.4B/2.8B

Mamba 2.8B is a large language model based on the state space model architecture, capable of competing with traditional Transformer models in handling information-dense data, such as language modeling.

The main innovations are as follows:

1. **Selective State Space Models (SSMs)**: Mamba introduces a selection mechanism by parameterizing SSM parameters based on the input. This allows the model to selectively propagate or forget information along the sequence length dimension based on the current token, enhancing its ability to focus on relevant information while discarding irrelevant data.

2. **Hardware-aware Parallel Algorithms**: To overcome the computational complexity introduced by selective state space models (SSMs), Mamba employs a hardware-aware algorithm that uses scanning rather than convolution to compute the model.

   > Scanning operations are more common in recursive computations, especially in models that need to adjust parameters dynamically based on input. In the Mamba model, the introduction of the selection mechanism means that the model parameters can change dynamically based on the input, which disrupts the conditions for using convolution. The scanning operation calculates the sequence state step by step in sequence order, allowing each step's computation to be dynamically adjusted based on the current input and previous state.

3. **Long Context Processing**: Capable of handling sequence lengths up to 1 million, performing well in audio processing and genomics.



### StripedHyena

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://www.together.ai/blog/stripedhyena-7b) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/togethercomputer/stripedhyena) 

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/togethercomputer/stripedhyena-65d8e6e77540dd1da932dbe1)

-  2023-12
-  **Pretrain Data Scale:** 2T
-  **Language Support:** Multiple
-  **Parameter Size:** 7B

The model series includes two main variants: StripedHyena-Hessian-7B and StripedHyena-Nous-7B. The [former](https://huggingface.co/togethercomputer/StripedHyena-Hessian-7B) is the base model, while the [latter](https://huggingface.co/togethercomputer/StripedHyena-Nous-7B) is the chat model.

StripedHyena adopts a hybrid architecture that combines gated convolutions and grouped-query attention mechanisms. The core component of the model is the state space model (SSM) layer, traditionally used for modeling complex sequences and time series data. The SSM layer can handle long sequence tasks more efficiently, reducing computational resource requirements and training faster on long sequences compared to classic Transformers.

StripedHyena supports training sequence lengths up to 32K, enabling it to handle longer prompts.





### YI

[![arXiv](https://img.shields.io/badge/arXiv-2403.04652-b31b1b.svg)](https://arxiv.org/abs/2403.04652) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/01-ai/Yi) 
[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/01-ai/yi-2023-11-663f3f19119ff712e176720f)

- **Date:** 2023-11
- **Pretrain Data Scale:**0. 8T～3T
- **Language Support:** Multiple
- **Parameter Size:** 6B/9B/34B

The Yi series includes foundational models with 6B, 9B, and 34B parameters, each with a default context window of 4K, extendable to 32K during inference.

The core highlights are as follows:

1. **High-Quality Data Preprocessing**: The Yi series models use a rigorous cleaning pipeline to ensure high-quality training data. This includes using heuristic rules and learned filters to remove low-quality and inappropriate content, ensuring the purity and relevance of the dataset.
2. **Improved Attention Mechanism**: The Yi models adopt an improved Grouped-Query Attention (GQA) mechanism, significantly reducing training and inference costs while being more efficient than traditional multi-head attention mechanisms.
3. **Multimodal Support**: The Yi series also includes multimodal models (Yi-VL), which can handle both text and image inputs, enabling multi-turn conversations and visual question answering.
4. **Better Chinese Language Support**: The Yi-34B performs well on three major Chinese benchmarks, CMMLU, E-Eval, and Gaokao, comparing favorably with chatGPT4.

> Principle of Grouped-Query Attention (GQA): In traditional multi-head attention mechanisms, each attention head has its own independent query (Q), key (K), and value (V) vectors. In GQA, query heads are divided into several groups, each sharing a single key (K) and value (V) vector. Specifically, if an attention layer has `H` query heads, these heads are divided into `G` groups (`G < H`), with each group sharing the same K and V vectors.
>
> Under the GQA mechanism, the number of key and value vector computations is reduced because multiple query heads within the same group share the same K and V. This reduces the number of matrix multiplications, thereby lowering computational complexity.





### Orca2
[![arXiv](https://img.shields.io/badge/arXiv-2311.11045-b31b1b.svg)](https://arxiv.org/pdf/2311.11045.pdf) 
[![Hugging Face collection](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/microsoft/orca-65bbeef1980f5719cccc89a3)

**Orca 2 is a finetuned version of LLAMA-2**. Orca 2’s training data is a synthetic dataset that was created to enhance the small model’s reasoning abilities. All synthetic training data was moderated using the Microsoft Azure content filters.

The paper provides a detailed explanation of how Orca, despite being a smaller model, can rival large language models like GPT-3.5 and even GPT-4.

- **Date:** 2023-11
- **Pretrain Data Scale:** same as LLAMA-2
- **Language Support:** en
- **Parameter Size:** 7B/13B



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



### Persimmon

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Phi%20AI-orange.svg)](https://www.adept.ai/blog/persimmon-8b) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/persimmon-ai-labs/adept-inference) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/adept/persimmon-8b-chat)

- **Date:** 2023-09
- **Pretrain Data Scale:** 0.737T
- **Language Support:** en
- **Parameter Size:** 8B

Persimmon-8B supports a context length of 16K, four times that of LLaMA2 and eight times that of GPT-3.

It adopts several architectural optimizations, including square ReLU activation functions and rotary positional encodings.

The model's input and output embeddings are optimized separately to avoid a full reduction in large embedding layer gradients, thereby improving training efficiency.



### Qwen

[![arXiv](https://img.shields.io/badge/arXiv-2309.16609-b31b1b.svg)](https://arxiv.org/abs/2309.16609) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/QwenLM/Qwen) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/Qwen)

Qwen optimize specific tasks through Instruction Fine-Tuning, such as programming language generation (CodeQwen), using Mixture of Experts (MoE) and sparse activation techniques.

- **Date:** 2023-08
- **Pretrain Data Scale:** 2.2T~3T(1.8B:2.2T;7B:2.4T;14B:3.0T)
- **Language Support:** en,zh
- **Parameter Size:** 0.5B/1.8B/4B/7B/14B/72B





### Llama2

[![arXiv](https://img.shields.io/badge/arXiv-2307.09288-b31b1b.svg)](https://arxiv.org/abs/2307.09288) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/meta-llama/llama)
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/meta-llama/llama-2-family-661da1f90a9d678b6f55773b)


The Llama 2 pretrained model shows significant improvements over the Llama 1 model, with a 40% increase in total training tokens and a longer context length of up to 4000 tokens. It also uses grouped-query attention to greatly accelerate inference speed for the 70B model. The Llama 2-Chat series, optimized for dialogue scenarios using Reinforcement Learning from Human Feedback (RLHF), outperforms most existing open models in extensive usability and safety tests, demonstrating performance comparable to ChatGPT in human evaluations.

- **Date:** 2023-07
- **Pretrain Data Scale:** 2T
- **Language Support:** en
- **Parameter Size:** 7B/13B/70B



### Falcon

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Falcon%20AI-orange.svg)](https://huggingface.co/blog/falcon-180b) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/falconry/falcon) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/tiiuae)

A large portion of the training data comes from [RefinedWeb](https://arxiv.org/abs/2306.01116), a new web dataset based on CommonCrawl. The model employs [**multiquery attention**](https://arxiv.org/abs/1911.02150). In the original multi-head attention scheme, each head has its own query, key, and value, whereas the multiquery attention scheme shares the same key and value across all heads. This technique has little impact on pretraining but significantly [enhances the scalability of inference](https://arxiv.org/abs/2211.05102). In fact, **this technique greatly reduces the memory footprint of the K,V cache during autoregressive decoding, cutting it down by 10-100 times** (the exact value depends on the model architecture), thereby significantly lowering the memory overhead of model inference. This reduction in memory overhead unlocks new optimization possibilities, such as using the saved memory to store historical conversations, making stateful inference possible.

- **Date:** 2023-07
- **Pretrain Data Scale:** 2T
- **Language Support:** en,fr
- **Parameter Size:** 1.3B/7.5B/40B/180B



### XGen

[![arXiv](https://img.shields.io/badge/arXiv-2309.03450-b31b1b.svg)](https://arxiv.org/abs/2309.03450) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/salesforce/xGen) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/Salesforce/xgen-7b-4k-base)

The XGen-7B model supports inputs up to 8K tokens. It is trained using standard dense attention and with up to 1.5T tokens, and it is fine-tuned on public domain instructional data. This makes it a versatile model suitable for standard-sized GPUs and mobile devices.

- **Date:** 2023-07
- **Pretrain Data Scale:** 1.37T
- **Language Support:** en
- **Parameter Size:** 7B











### Zephyr
[![arXiv](https://img.shields.io/badge/arXiv-2310.16944-b31b1b.svg)](https://arxiv.org/abs/2310.16944) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/huggingface/alignment-handbook) 
- **Date:** 2023-05
- **Pretrain Data Scale:** According to LLM
- **Language Support:** en
- **Parameter Size:** 7B

The Zephyr series of large language models employs diverse preference optimization techniques to better align with specific user preferences or task requirements. This series includes three models, each using different preference optimization algorithms and base LLMs.

> Preference optimization techniques can ensure that generated outputs better meet expectations, **reduce undesirable outputs**, and significantly enhance the model's customization capabilities.

#### Zephyr-7B

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/HuggingFaceH4/zephyr-7b-6538c6d6d5ddd1cbb1744a66)

Zephyr-7B-β is the first model in the Zephyr series, fine-tuned based on [Mistralai/Mistral-7B-v0.1](https://link.zhihu.com/?target=https%3A//huggingface.co/mistralai/Mistral-7B-v0.1) using the **Direct Preference Optimization (DPO)** algorithm.

Additionally, this model utilizes knowledge distillation, where a smaller "student" model learns and replicates the performance of a larger "teacher" model. This allows Zephyr-7B to retain the capabilities of a larger model while achieving higher computational efficiency, making it easier to deploy on devices with limited computational resources.

The datasets used are UltraChat and UltraFeedback:

- UltraChat is a synthetic dialogue dataset generated by ChatGPT.
- UltraFeedback includes various prompts and responses, annotated by GPT-4.

> Direct Preference Optimization (DPO) aligns preferences by directly maximizing the probability of the preferred responses generated by the model. The DPO algorithm optimizes the probability of the preferred responses without the need for a reference model, simplifying the training process.

#### Zephyr ORPO

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/HuggingFaceH4/zephyr-orpo-6617eba2c5c0e2cc3c151524)

Zephyr-ORPO-141B-A35b-v0.1 is an expert mixture (MoE) model with 141B total parameters and 39B active parameters, fine-tuned based on [Mixtral-8x22B-v0.1](https://huggingface.co/mistral-community/Mixtral-8x22B-v0.1) using the [Odds Ratio Preference Optimization (ORPO)](https://huggingface.co/papers/2403.07691) algorithm for preference optimization. ORPO achieves high performance without needing the SFT step, making it far more computationally efficient than methods like DPO and PPO.

The ORPO model also effectively reduces undesirable responses through a dynamic penalty mechanism, ensuring high quality and applicability of the output content.

> **Odds Ratio Preference Optimization (ORPO)** optimizes by calculating the odds ratio of preferred to non-preferred responses, ensuring the model is more inclined to generate preferred responses.

#### Zephyr-7B Gemma

[![Hugging Face collections](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-collections-blue)](https://huggingface.co/collections/HuggingFaceH4/zephyr-7b-gemma-65e1fd82d26b426e3e63d956)

This is a fine-tuned version of [google/gemma-7b](https://huggingface.co/google/gemma-7b) on the HuggingFaceH4/deita-10k-v0-sft dataset, also using the DPO preference optimization algorithm.



### Pythia

[![arXiv](https://img.shields.io/badge/arXiv-2304.01373-b31b1b.svg)](https://arxiv.org/abs/2304.01373) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/EleutherAI/pythia) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/collections/EleutherAI/pythia-scaling-suite-64fb5dfa8c21ebb3db7ad2e1)

- **Date:** 2023-04
- **Pretrain Data Scale:** 10B
- **Language Support:** en
- **Parameter Size:** 130M/370M/790M/1.4B/2.8B

Pythia *Scaling Suite* is a collection of models developed to facilitate interpretability research. It is a suite of 16 LLMs, all trained on public data seen in the exact same order and ranging in size from 70M to 12B parameters.

> The large language model (LLM) suite is a series of language models designed for scientific research. These models emphasize consistency and reproducibility in their design and implementation, aiming to allow researchers to deeply analyze and understand the behavior and changes of large language models during training and scaling processes.

Pythia contains two sets of eight models with sizes of 70M, 160M, 410M, 1B, 1.4B, 2.8B, 6.9B, and 12B. For each size, there are two models: one trained on the Pile, and one trained on the Pile after the dataset has been globally deduplicated. All 8 model sizes are trained on the exact same data, in the exact same order.

> The Pile is a large, open-source English text dataset designed specifically for training large language models. It consists of 22 different, high-quality sub-datasets, including texts from books, academic papers, legal documents, online Q&A, programming code, and movie subtitles. It is widely used for training large language models, including autoregressive transformers. For more details: [click here](https://pile.eleuther.ai/).

The Pythia suite is the only publicly released LLM suite that meets the following three key characteristics:

1. Models cover multiple orders of magnitude in scale.
2. All models are trained on the same data in the same order.
3. Data and intermediate checkpoints are available for public research use.

The authors also conducted three case studies in language modeling research:

1. **How data bias affects learning behavior**: The study shows that appropriate interventions in language models can reveal that the frequency of pronoun occurrences in the data affects the model's learning bias. The research also proposes a controllable method to analyze and mitigate model bias.
2. **Does training order affect memory**: Researchers found that Poisson models fit the data well, indicating that training order has little impact on memory. The model shows that memory sequences do not appear more densely at the beginning or end of the training process, but rather, an approximately equal number of memory sequences are distributed between checkpoints.
3. **Does the frequency of pre-training terms affect task performance throughout the training process**: This correlation is more pronounced in larger models. Smaller models struggle to achieve accurate results on these tasks, even in the later stages of training, indicating that these models cannot successfully learn these tasks regardless of the frequency of relevant information in the training data.







### Vicuna

[![AI Blog](https://img.shields.io/badge/AI%20Blog-Vicuna%20AI-orange.svg)](https://lmsys.org/blog/2023-03-30-vicuna/) 
[![GitHub](https://badges.aleen42.com/src/github.svg)](https://github.com/lm-sys/FastChat) 
[![Hugging Face model](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-models-blue)](https://huggingface.co/lmsys)

1. **Memory Optimization**: To meet Vicuna's requirements for handling long contexts, its maximum context length was increased from Alpaca's 512 to 2048, significantly increasing the demand for GPU memory. To address this issue, researchers adopted gradient checkpointing and FlashAttention techniques to alleviate memory pressure.
2. **Multi-turn Conversations**: By adjusting the training loss to accommodate the needs of multi-turn conversations, the calculation of training loss is based solely on the chatbot's output.
3. **Cost Reduction through Spot Instances**: The dataset size increased 40 times and the sequence length increased 4 times, posing greater challenges to training. To reduce costs, researchers used SkyPilot-hosted Spot instances, taking advantage of automatic recovery from preemption and automatic region switching, thereby using the more cost-effective Spot instances. This strategy reduced the training cost of the 7B model from \$500 to approximately \$140, and the training cost of the 13B model from about \$1000 to \$300.

- **Date:** 2023-03
- **Pretrain Data Scale:** 1.4T
- **Language Support:** en,zh
- **Parameter Size:** 7B/13B/33B





## Model Evaluation Platforms

### OpenLLM Leaderboard by Hugging Face [[Leaderboard]](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard)

The OpenLLM Leaderboard by Hugging Face is a platform designed to track, rate, and evaluate open-source large language models (LLMs) and chatbots. This leaderboard provides a centralized platform.

[Open LLM Leaderboard](https://huggingface.co/spaces/HuggingFaceH4/open_llm_leaderboard) is actually just a wrapper running the open-source benchmarking library [Eleuther AI LM Evaluation Harness](https://github.com/EleutherAI/lm-evaluation-harness) created by the [EleutherAI non-profit AI research lab](https://www.eleuther.ai/), famous for creating [The Pile](https://pile.eleuther.ai/) and training [GPT-J](https://huggingface.co/EleutherAI/gpt-j-6b), [GPT-Neo-X 20B](https://huggingface.co/EleutherAI/gpt-neox-20b), and [Pythia](https://github.com/EleutherAI/pythia). A team with serious credentials in the AI space! (Citation from Hugging Face blog)

### Chatbot Arena by LMSYS and SkyLab [[Chatbot Arena]](https://arena.lmsys.org/)

Main features of Chatbot Arena:

1. **Arena Battle**: In Chatbot Arena, users can select two different anonymous models (such as ChatGPT, Claude, Llama, etc.) and compare them. In a secure competition environment, users can ask questions and evaluate the responses of the two models, voting to decide which model performs better. This comparison process can continue for multiple rounds until a final winner is determined. To ensure fairness, if a specific model's identity is revealed during any round, the results of that round's vote will be excluded.
2. **Direct Chat**: Chatbot Arena offers a real-time chat feature that allows users to directly interact with the selected model. Whether users choose text or visual chat modes, they can receive immediate feedback from the model.
3. **Leaderboard**: Chatbot Arena uses a ranking system based on the Elo rating system, analyzing the voting results of over 300,000 human users to evaluate the rankings of various LLMs. This allows users to easily see which models are currently leading and identify the top performers in the LLM field.




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


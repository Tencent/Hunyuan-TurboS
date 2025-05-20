# Hunyuan-TurboS: Advancing Large Language Models through Mamba-Transformer Synergy and Adaptive Chain-of-Thought

## Abstract 
As Large Language Models (LLMs) rapidly advance, we introduce Hunyuan-TurboS, a novel large hybrid Transformer-Mamba Mixture of Experts (MoE) model. It synergistically combines Mamba's long-sequence processing efficiency with Transformer's superior contextual understanding. Hunyuan-TurboS features an adaptive long-short chain-of-thought (CoT) mechanism, dynamically switching between rapid responses for simple queries and deep "thinking" modes for complex problems, optimizing computational resources. Architecturally, this 56B activated (560B total) parameter model employs 128 layers (Mamba2, Attention, FFN) with an innovative AMF/MF block pattern. Faster Mamba2 ensures linear complexity, Grouped-Query Attention minimizes KV cache, and FFNs use an MoE structure. Pre-trained on 16T high-quality tokens, it supports a 256K context length and is the first industry-deployed large-scale Mamba model. Our comprehensive post-training strategy enhances capabilities via Supervised Fine-Tuning (3M instructions), a novel Adaptive Long-short CoT Fusion method, Multi-round Deliberation Learning for iterative improvement, and a two-stage Large-scale Reinforcement Learning process targeting STEM and general instruction-following. Evaluations show strong performance: overall top 7 rank on LMSYS Chatbot Arena with a score of 1356, comparable to leading models like DeepSeek-R1 (1355) and o4-mini-2025-04-16 (1345). TurboS also achieves average 77.9\% across 23 automated benchmarks. Hunyuan-TurboS balances high performance and efficiency, offering substantial capabilities at lower inference costs than many reasoning models, establishing a new paradigm for efficient large-scale pre-trained models.

![Intro_P1](Figures/intro_p_v1.png)



## Technical Details

Full technical details can be found in our [technical report](Hunyuan_TurboS_Report.pdf).

## Human Evaluation: LMSYS Chatbot Arena

We report the performance of our model Hunyuan-TurboS-20250416 on LMSYS Chatbot Arena, and the detailed results are as following:

1.  Hunyuan-TurboS-20250416 obtains an overall score of **1356**, is among the **top 7** best models in total 239 models, and outperforming leading reasoning models like DeepSeek-R1, Qwen3-235B-A22B, and o4-mini-2025-04-16.

2.  Hunyuan-TurboS-20250416 achieves **top 1** in **Chinese**, **French**, **Spanish**, and **top 2** in **Korean** languages. 
3.  Hunyuan-TurboS-20250416 achieves **top 5** in various main Arena tasks, such as **Hard Prompts**, **Creative Writing**, **Multi-Turn**, and **Longer Queries**.

![Intro_P1](Figures/table3.png)


## Full Evaluation Results
We present the evaluation results across diverse tasks spanning math, reasoning, code, knowledge, Chinese, alignment, and instruction following domains.

![Intro_P1](Figures/table4.png)




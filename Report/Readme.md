# Hunyuan-TurboS: Advancing Large Language Models through Mamba-Transformer Synergy and Adaptive Chain-of-Thought


<p align="center">
  <img src="Figures/hunyuan_v1.png" alt="Intro_P1" width="30%">
</p>

## Introduction

We are excited to introduce **Hunyuan-TurboS**, a novel large hybrid Transformer-Mamba mixture-of-experts (MoE) model that sets new standards in efficiency and performance. Hunyuan-TurboS cleverly combines the long-sequence processing efficiency of the Mamba architecture with the superior contextual understanding of the Transformer architecture.

The model features an adaptive long-short chain-of-thought (CoT) mechanism, allowing it to dynamically switch between rapid responses for simple queries and deep "thinking" modes for complex problems. This innovation optimizes computational resource usage while maintaining high performance across a wide range of tasks.

Hunyuan-TurboS has achieved remarkable results, including a score of **1355** on the LMSYS Chatbot Arena, placing it in the **top 10** models. It excels in math, multi-turn conversations, and longer queries, demonstrating its powerful reasoning capabilities and efficiency.

![Intro_P1](Figures/Intro_P1.png)

## Key Features

### Mamba Architecture Integration

Hunyuan-TurboS leverages the Mamba architecture for linear complexity in long-sequence processing, ensuring efficient handling of extensive contextual information. This makes it particularly suitable for tasks requiring long-context understanding and reasoning.

### Top 10 LMSYS Chatbot Arena Ranking

With a score of **1355**, Hunyuan-TurboS ranks **8th** on the LMSYS Chatbot Arena leaderboard. It outperforms many industry-leading models in blind, side-by-side human evaluations, showcasing its strong comprehensive capabilities.

### Adaptive Long-Short Chain-of-Thought Mechanism

The model employs an innovative adaptive long-short CoT mechanism. For simple questions, it activates a "no thinking" mode to deliver quick responses with minimal computational cost. For complex problems, it switches to a "thinking" mode, utilizing deep reasoning methods such as step-by-step analysis and self-reflection to provide highly accurate answers.

### Fast Inference Speed

Hunyuan-TurboS achieves impressive performance while maintaining fast inference speeds. Its optimized hybrid architecture and efficient computational strategies ensure low inference costs, making it more economical than many reasoning models.

## Model Details

### Model Architecture

Hunyuan-TurboS is a hybrid model combining Transformer, Mamba2, and Feed-Forward Network (FFN) components. It consists of 128 layers, with a total of 560B parameters and 56B activated parameters. The model uses an innovative AMF/MF block pattern to balance performance and efficiency.
![Intro_P1](Figures/TurboS.png)



### Pre-training and Post-training

- **Pre-training**: The model was pre-trained on a dataset of 16T high-quality tokens, supporting a context length of up to 256K. It employs techniques such as annealing and curriculum-based long-context extension to enhance its capabilities.
- **Post-training**: Our comprehensive post-training strategy includes Supervised Fine-Tuning, Adaptive Long-Short CoT Fusion, Multi-round Arena Learning, and a two-stage Large-scale Reinforcement Learning process. This strategy significantly improves the model's capabilities across various domains.
![Intro_P1](Figures/data_process_v1.png)

![Intro_P1](Figures/post_train_v1.png)


## Getting Started

### Usage Recommendations

To achieve optimal performance when using Hunyuan-TurboS: Set the temperature between 0.5-0.7 (0.6 is recommended) to avoid endless repetitions or incoherent outputs.


## Evaluation Results

Hunyuan-TurboS demonstrates state-of-the-art performance across multiple benchmarks:

![Intro_P1](Figures/eval_bench_v1.png)



## License

Hunyuan-TurboS is licensed under the Proprietary License. 

## Citation

If you use Hunyuan-TurboS in your research, please cite the following paper:

```
@misc{hunyuanai2025hunyuan-turbos,
      title={Hunyuan-TurboS: Advancing Large Language Models through Mamba-Transformer Synergy and Adaptive Chain-of-Thought},
      author={Tencent Hunyuan Team},
      year={2025},
      eprint={2505.19},
      archivePrefix={arXiv},
      primaryClass={cs.CL},
      url={https://example.com/hunyuan-turbos-paper},
}
```

## Contact

For any questions or feedback, please contact us at service@hunyuan.com.

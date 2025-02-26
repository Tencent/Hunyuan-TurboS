# 混元TurboS - 探索Hybrid-Transformer-Mamba 在大规模MoE模型上的实现

## 简介
传统的纯 Tranformer 结构大模型，受限于其 O(N^2) 计算复杂度和 KV-Cache 问题，长文训练和推理成本都非常高。我们采取了高效线性结构 Mamba和 Transformer 的混合架构，成功推出了业界首个超大规模Hybrid-Transformer-Mamba MoE大模型Hunyuan-TurboS，该模型具有 Mamba 高效处理长序列能力，还保留 Transformer 擅于捕捉复杂上下文和长距离依赖的能力。相比起上一代 Turbo 模型，Hunyuan-TurboS结构在模型效果有一定提升的同时，可以将平均推理成本降低到 1/7。

后训练阶段，我们汲取了慢思考模型强大的推理能力，将长短思维链融合后大幅提升了数学、代码、逻辑推理等任务效果。通过更精细的指令覆盖和强化策略，显著提升了指令遵循和agent规划执行能力。同时，我们针对英文数据进行了质量优化和提升，整体提升了英文通用效果。我们将奖励模型升级为奖励系统，扩展支持基于规则和一致性验证的奖励打分，以及代码沙盒验证反馈，显著提升了理科场景的效果；在问答、创作等场景，支持了基于生成式的奖励反馈有效避免reward hacking并提升OOD泛化效果。

最终，Hunyuan-TurboS在Math、Reasoning、Alignment等基准中表现优于GPT4O-0806、DeepSeek V3和其他开源模型，同时在包括MMLU-Pro在内的Knowledge也表现出了有竞争力的成果。

## 模型效果
![image](https://github.com/user-attachments/assets/65f3b0b2-ef61-466b-a3c4-e154dde93e3c)

![image](https://github.com/user-attachments/assets/d653fca6-26eb-49d8-8997-6b4c35154511)



<link rel="stylesheet" href="/llm.hunyuan.turbo-s/assets/css/custom-theme.css">

# 腾讯推出新一代快思考模型混元 Turbo S，将在腾讯元宝逐步灰度上线

_腾讯混元Turbo S模型已在腾讯云官网上架，开发者和企业用户可以通过API调用，今天开始在腾讯元宝灰度上线，供广大用户使用和体验。_

<br>
2月27日，腾讯混元自研的快思考模型Turbo S正式发布。区别于Deepseek R1、混元T1等需要“想一下再回复”的慢思考模型，混元Turbo S能够实现“秒回”，吐字速度提升一倍，首字时延降低44%，同时在知识、数理、创作等方面也有突出表现。通过模型架构创新，Turbo S 部署成本也大幅下降，持续推动大模型应用门槛降低。

有研究表明，人类约90%—95%的日常决策依赖直觉，快思考正如人的“直觉”，为大模型提供了通用场景下的快速响应能力，而慢思考更像理性思维，通过分析逻辑提供解决问题思路。快思考和慢思考的结合和补充，可以让大模型更智能、更高效地解决问题。

在业界通用的多个公开Benchmark上，腾讯混元 Turbo S 在知识、数学、推理等多个领域展现出对标 DeepSeek V3、GPT 4o、Claude3.5等业界领先模型的效果表现。

<img width="950" alt="image" src="https://github.com/user-attachments/assets/4a0f5438-bc2d-40f9-be82-f1769aed15fb" />

<br>

<img width="950" alt="image" src="https://github.com/user-attachments/assets/d8b80f17-213f-41dd-a4ff-893c85c5bd79" />

<sub>*表格中，其它模型的评测指标来自官方评测结果，官方评测结果中不包含部分来自混元内部评测平台<sub>

<br>
据介绍，通过长短思维链融合，腾讯混元Turbo S 在保持文科类问题快思考体验的同时，基于自研混元 T1 慢思考模型合成的长思维链数据，显著改进了理科推理能力，实现模型整体效果提升。

架构方面，通过创新性地采用了Hybrid-Mamba-Transformer 融合模式，混元Turbo S有效降低了传统Transformer结构的计算复杂度，减少了KV-Cache缓存占用，实现训练和推理成本的下降。新的融合模式突破了传统纯 Transformer 结构大模型面临的长文训练和推理成本高的难题，一方面发挥了Mamba 高效处理长序列的能力，也保留 Transformer 擅于捕捉复杂上下文的优势，构建了显存与计算效率双优的混合架构，这是工业界首次成功将Mamba架构无损地应用在超大型MoE模型上。

作为旗舰模型，Turbo S未来将成为腾讯混元系列衍生模型的核心基座，为推理、长文、代码等衍生模型提供基础能力。基于Turbo S，通过引入长思维链、检索增强和强化学习等技术，腾讯自研了推理模型 T1，该模型已在腾讯元宝上线，用户可以选择Deepseek R1 或腾讯混元T1模型进行回答。腾讯混元表示，正式版的腾讯混元T1模型API也将很快上线，对外提供接入服务。

开发者和企业用户已经可以在腾讯云上通过API调用腾讯混元Turbo S，即日起一周内免费试用。定价上，Turbo S 输入价格为0.8元/百万tokens，输出价格为2元/百万tokens，相比前代混元Turbo模型价格下降数倍。

<br>

腾讯混元turbos模型免费[试用申请](https://cloud.tencent.com/apply/p/i2zophus2x8)

扫码体验：

![image](https://github.com/user-attachments/assets/09958261-98ae-435a-ac9a-ba7a0982a728)




<link rel="stylesheet" href="/llm.hunyuan.turbo-s/assets/css/custom-theme.css">

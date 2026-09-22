---
title: 'RLinf × SGLang：Cosmos3 从模型微调到高效评测的全流程集成实践分享'
date: 2026-09-20
---

随着具身智能模型不断演进，模型本身的能力只是完整开发链路的一部分。对于一个新的 World Action Model（WAM）而言，从模型接入、训练，到推理和仿真评测，都需要一套能够快速适配并高效运行的基础设施。

RLinf 此前已经支持 DreamZero 等世界模型。此次，我们进一步将 NVIDIA Cosmos 3 集成到 RLinf，并结合 SGLang 作为推理后端，打通从模型 SFT、推理服务到仿真评测的完整流程。基于 RLinf 完成 Cosmos3-Nano SFT，训练精度与官方实现对齐；同时显著提升 Cosmos3 仿真评测吞吐，通过增强 SGLang 多 batch 推理及流水线并行评测，相比直接集成 SGLang 实现了 3.33 倍性能提升。

本文以 Cosmos3-Nano 集成为例，介绍从模型微调到高效并行评测的全流程集成过程中的关键技术设计，以及 RLinf 如何通过流水化调度进一步提升模型评测效率。

- [查看详细报道](https://mp.weixin.qq.com/s/4w-085A4Yk5WJk2wNGpdMw?scene=1&click_id=2)
- [SGLang 官方推送](https://www.sglang.io/blog/rlinf-sglang-cosmos3)

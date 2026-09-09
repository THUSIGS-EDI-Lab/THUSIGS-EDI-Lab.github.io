---
title: 'RLinf 精度对齐 + 百度百舸全链路优化：OpenPI PyTorch 训练吞吐提升 2.37 倍'
date: 2026-08-21
---

经过 RLinf 的精度对齐与百度百舸的 AI Infra 全链路工程优化，OpenPI Pi0.5 在国内主流 GPU（无 NVLink、无 HPN）环境上实现了显著的训练加速。

- 单机 8 卡训练吞吐从 74.20 sps 提升至 175.57 sps，达到 2.37 倍提升；
- 单个 epoch 训练时间从 61.4 分钟缩短至 26.0 分钟；
- 训练精度与基线完全一致；
- 32 机 256 卡规模下线性扩展比保持 91% 以上，集群算力得到充分释放。

[查看详细报道](https://mp.weixin.qq.com/s/4jWQ-FX9AmoY-EXv5sbBdQ?scene=1&click_id=9)

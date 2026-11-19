---
layout: page
title: Jagged Robustness
description: Audit the impact of quantization on capability and safety domains including model safeguards, instruction-following, ethics and bias through adversarial suffix attacks and benchmarks
importance: 1
img: assets/img/jagged_robustness.png
github: https://github.com/LucianoXu/QuantBeyoundEfficiency/tree/main
paper: https://github.com/ramneekagn/jagged_robustness_workshop/blob/main/llm_robustness_paper.pdf
---
Quantization enables efficient inference in language
models through model parameter compression. This work audits
the impact of quantization on capability and safety domains
including model safeguards, instruction-following, ethics and bias.
Through benchmarks, we find that model safeguards and bias
can degrade under quantization, while other capabilities such
as truthfulness remain more stable in Qwen3-4B. We define this
uneven transfer of LLM capabilities under quantization as Jagged
Robustness. We find multiple factors driving Jagged Robustness:
task complexity, evaluation method and generation coherence.
Moreover, we verify the degradation of model safeguards by
observing increased compliance with unsafe requests under
quantization, and demonstrate universal adversarial suffix attacks
that are benign for the full model but jailbreak quantized
models. The findings indicate that it is risky to assume that the
performance and robustness can transfer evenly across different
capability domains from full models to quantized models.
---
layout: page
title: LLM Safety Harness
description: Safety scaffold around LLMs with BERT models auditing input and outputs. Linear probes used for inner detection. All of them combined with an AND ensemble. 
importance: 2
img: assets/img/architecture_llmsafetyharness.png
github: https://github.com/ramneekagn/SafeguardLLM
category: work
---
A harness is defined as a software scaffold around an LLM. Unlike agent harnesses, where the scaffolds are RAGs or connections to tool calls, our method connects LLMs to various detectors. We use BERT classifiers to detect input and output text, while simultaneously auditing the models' internals using linear probes. We evaluated the models on various metrics. The final decision on whether an input or generation is flagged as a jailbreak is made by AND ensemble from all the classifiers.

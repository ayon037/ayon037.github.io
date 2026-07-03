---
title: "ProfilingAgent: Profiling-Guided Agentic Reasoning for Adaptive Model Optimization"
collection: publications
category: manuscripts
permalink: /publication/2025-09-06-ProfilingAgent
date: 2025-09-06
venue: 'IEEE Computational Intelligence Society (CIS)'
status: 'Under review at'
paperurl: 'https://arxiv.org/abs/2509.05584'
citation: 'Mohiuddin Bilwal, Co-Author. (2025). &quot;ProfilingAgent: Profiling-Guided Agentic Reasoning for Adaptive Model Optimization.&quot; <i>IEEE Computational Intelligence Society (CIS)</i>.'
---
Foundation models face growing compute and memory bottlenecks, hindering deployment on resource-limited platforms without optimization. While model compression techniques like pruning and quantization are widely used, most ex- isting approaches rely on uniform heuristics or rule-based strategies that ignore architectural and runtime heterogeneity. Profiling tools have been developed to expose such bottlenecks by capturing metrics like per-layer latency, memory usage, and compute cost; however, these insights are rarely integrated into automated compression pipelines. In this paper, we propose ProfilingAgent, a profiling-guided agentic approach that leverages large language models (LLMs) to automate model compression through structured pruning and post-training dynamic quan-
tization. Our modular pipeline consists of a multi-agent system that leverages both static (e.g., MACs, parameter counts) and dynamic (e.g., latency, memory usage) profiling signals to generate architecture-specific compression strategies. Unlike heuristic baselines for pruning and quantization, our LLM-guided agents reason over profiling traces to produce layer-wise decisions tailored to performance bottlenecks. Experiments conducted on benchmark datasets, such as ImageNet 1K, CIFAR-10 and CIFAR-100, utilizing ResNet-101, ViT-B/16, Swin-B, and DeiT-
B/16, demonstrate that our approach to pruning maintains competitive or even improved accuracy (with accuracy drops of about 1% on ImageNet-1K, and gains of up to +2% for ViT-B/16 on smaller datasets without any post-pruning fine-tuning), while quantization achieves memory savings of up to 74% with accuracy drops below 0.5%. Furthermore, our quantization strategy consistently delivers inference speedups of up to 1.74×, effectively reducing latency while preserving performance. Comparative studies with GPT-4o and GPT-4-Turbo underscore the impact of LLM reasoning quality on iterative pruning efficacy. These results establish agentic systems as a scalable solution for profiling-guided model optimization.
---
layout: default
---

# Overview
<p style='text-align: justify;'>
Large Language Models (LLMs) trained on large corpora of texts have attracted significant attention in recent years with their ability to solve tasks with few supervised examples. These few-shot models have shown state-of-the-art success across NLP tasks (Entity Recognition), language translation, standardized exams (SAT, AP exams, Medical Knowledge), coding challenges (LeetCode), as well as in subjective domains such as chatbots. All of these domains involve bootstrapping a single LLM referred to as a foundation model with examples of specific knowledge from the associated task. The process of updating a model with limited domain-specific data is known as fine-tuning. However, the costs of accessing, fine-tuning and querying foundation models to perform new tasks are large. Given these costs, access to performant LLMs has been gated behind expensive and often proprietary hardware used to train models, making them inaccessible to those without substantial resources. 

Our goal is to democratize access to language models and address three major issues:

1. Lack of transparency around model training methods leads to a majority of models being not reproducible. Preprint. Under review. 

2. The absence of a standard benchmark to evaluate these models side-by-side. 

3. Insufficient access to dedicated hardware prevents widespread availability and usage of these models. 

Here we present a LLM efficiency challenge, to tackle these three challenges and democratize access to state of the art LLMs. Specifically, we introduce a challenge for the community to adapt a foundation model to specific tasks by fine-tuning on **a single GPU** of either 4090 or A100 within a **24-hour** (1-day) time frame, while maintaining high accuracy for these desired tasks. Beyond providing a suite of evaluation tasks, we will perform extensive analysis on each submission to study accuracy and computational performance tradeoffs at commodity hardware scales. The outcome of this competition is to distill the insights and lessons into a set of well documented steps and easy-to-follow tutorials. The ML community will have documentation on how to achieve the same performance as winning entries, which will serve as the starting point to help them build their own LLM solutions.

</p>
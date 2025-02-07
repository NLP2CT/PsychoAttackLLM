# Priming Attacks
## Abstract

Large language models (LLMs) have significantly influenced various industries but suffer from a critical flaw, the potential sensitivity of generating harmful content, which poses severe societal risks. We developed and tested novel attack strategies on popular LLMs to expose their vulnerabilities in generating inappropriate content. These strategies, inspired by psychological phenomena such as the **"Priming Effect"**, **"Safe Attention Shift"**, and **"Cognitive Dissonance"**, effectively attack the models' guarding mechanisms.

Our experiments achieved an attack success rate (ASR) of 100% on various open-source models, including Meta's Llama-3.2, Google's Gemma-2, Mistral's Mistral-NeMo, Falcon's Falcon-mamba, Apple's DCLM, Microsoft's Phi3, and Qwen's Qwen2.5, among others. Similarly, for closed-source models such as OpenAI's GPT-4o, Google's Gemini-1.5, and Claude-3.5, we observed an ASR of at least 95% on the AdvBench dataset, which represents the current state-of-the-art.

This study underscores the urgent need to reassess the use of generative models in critical applications to mitigate potential adverse societal impacts.

## Main Results
Furthermore, we conducted benchmark tests on the latest large language models (LLMs) as of October 2024 using the **AdvBench** dataset, employing both closed-source and open-source models with the proposed strategy. As shown in **Table: Newest**, the results demonstrate that the **Priming Attack** method achieved a 100% attack success rate (ASR) on open-source models and nearly 100% on closed-source models. This indicates that current LLMs remain highly susceptible to such attacks. 

## Comparison of Close-Source and Open-Source Target Models

The table below presents the Attack Success Rate (ASR) for models when attacked once (1 tried) and multiple times.

| **Model**                    | **1 tried** | **≤3 tried** |
|------------------------------|-------------|--------------|
| GPT-3.5-turbo                 | 0.910       | 1.000        |
| GPT-4-0613                    | 0.919       | 0.996        |
| GPT-4o-2024-05-13             | 0.856       | 0.958        |
| Gemini-1.5-pro                | 0.913       | 0.954        |
| Claude-3-opus                 | 0.810       | 0.998        |
| Claude-3.5-Sonnet             | 0.967       | 0.979        |
| **Llama3-8B-Instruct**        | 0.987       | 1.000        |
| Llama-3.1-8B-Instruct         | 0.992       | 1.000        |
| Llama-3.2-3B-Instruct         | 0.967       | 1.000        |
| Codestral-Mamba-7B-v0.1       | 0.979       | 1.000        |
| Mixtral-Nemo-Instruct         | 0.992       | 1.000        |
| Qwen2-7B-Instruct             | 1.000       | -            |
| Qwen2-57B-A14B-Instruct       | 1.000       | -            |
| Qwen2.5-7B-Instruct           | 0.996       | 1.000        |
| Qwen2.5-32B-Instruct          | 0.996       | 1.000        |
| Gemma-2-it-9b                 | 0.996       | 1.000        |
| Glm-4-9B-chat                 | 0.994       | 1.000        |
| Phi-3-mini-128k-instruct      | 0.987       | 1.000        |
| DCLM-7b-it                    | 0.992       | 1.000        |
| Falcon-mamba-7b-Instruct      | 0.992       | 1.000        |

## Future Updates

Other parts of this repository will be updated in future releases.

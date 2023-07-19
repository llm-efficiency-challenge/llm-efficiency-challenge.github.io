---
layout: default
---

<p style='text-align: justify;'>

To participate in this competition, you must start with a base model from our approved list, utilize only open-source data, and limit your fine-tuning to a single **24-hour** period. This fine-tuning should be carried out on just one graphics card, which must be either the **NVIDIA 4090** or the **NVIDIA A100**.
Our competition will feature two hardware tracks: the **NVIDIA 4090 track**  and  the **NVIDIA A100 track**, and each track will be evaluated separately.

</p>

## Approved Base models:

<p style='text-align: justify;'>
The starting model for the competition should be an open base model without instruction-tuning. Examples of licenses we'll accept are [MIT](https://spdx.org/licenses/MIT.html) or [Apache 2](https://www.apache.org/licenses/LICENSE-2.0)). We're also happy to discuss other licenses on a case by case basis, for example per community interest we'll accept the [LLAMA 2 community license agreement](https://github.com/facebookresearch/llama/blob/main/LICENSE) if you've requested and been approved for a [download link](https://ai.meta.com/resources/models-and-libraries/llama-downloads/). All sizes of the common autoregressive and autoencoder base models listed below are allowed. 

</p>

* Falcon
* LLaMA or Llama 2
* OpenLLaMA
* Red Pajama Base (not instruction tuned models)
* MPT
* OPT
* Bloom
* GPT Neo, J, NeoX, Pythia
* GPT2
* T5 (not Flan-T5)
* BART
* DeBERTa
* RoBERTa
* BERT
* ALBERT
* DistilBERT
* Electra
* UL2


If you plan to use an open-source base model family not listed here, please reach out to us and we will consider adding it to the list. Please respect the honor system in place for this competition, and acquire your base model through legitimate channels only. (i.e. No pirated LLaMA weights). Any submissions that use base models obtained through illicit means will be disqualified. 

## Datasets:

<p style='text-align: justify;'>
You are welcome to use any open sourced dataset. For example:
</p>

* [Databricks-Dolly-15](https://huggingface.co/datasets/databricks/databricks-dolly-15k)
* [OpenAssistant Conversations Dataset (oasst1)](https://huggingface.co/datasets/OpenAssistant/oasst1)
* [Alpaca Libre](https://github.com/mobarski/alpaca-libre)

<br>

<p style='text-align: justify;'>
Under no circumstances should you use data that infringes upon data usage agreements, copyright laws, or privacy policies. This means you should not use datasets that utilize generated content, whether in the form of instructions/prompts or results/answers from another LLM. If you opt to create your own dataset, it must be open-sourced and readily accessible to the general public at the time of submission.
</p>

<br>

## Evaluation:

<p style='text-align: justify;'>

The evaluation process in our competition will be conducted in two stages. In the first stage, we will run a subset of HELM benchmark along with a set of secret holdout tasks. The holdout tasks will consist of logic reasoning type of multiple-choice Q&A scenarios as well as conversational chat tasks. Submissions will be ranked based on their performance across all tasks. The ranking will be determined by the geometric mean across all evaluation tasks. This score will be shown in the leaderboard 

<br><br>

$$\text{score} = \Pi ( \text{mean-win-rate(\text{task})} )$$

<br><br>

After the competition is closed on September 30th 2023, we will contact the top 3 teams with the highest scoring models in each hardware category, requesting that they submit all necessary code and data to reproduce their model, starting from their chosen open-source base model. We will then replicate their entire process, to ensure it is repeatable and same results can be achieved with 24 hours using a single GPU. If the top-scoring model cannot be reproduced under these imposed conditions, we will move on to consider the next highest-scoring model in the hardware category, we will continue this process until a reproducible and high-performing model is selected, or we exhaust all potential options and declare no winners for the category.

</p>

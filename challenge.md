---
layout: default
---

# Large Language Model Efficiency Challenge:<br>1 LLM + 1GPU + 1Day

<p>Here we present a LLM efficiency challenge, to tackle some of the main challenges in LLMs and democratize access to state of the art LLMs. Specifically, we introduce a challenge for the community to adapt a foundation model to specific tasks by fine-tuning on a single GPU within  a 24-hour (1-day) time frame, while maintaining high accuracy for these desired tasks.</p>

<p>Beyond providing a suite of evaluation tasks, we will perform extensive analysis on each submission to study accuracy and computational performance tradeoffs at commodity hardware scales.</p>

## Important Dates

<table class="foo">
    <tr>
        <td width="50%"><b>Challenge Start</b></td>
        <td width="50%">May 31st, 2023</td>
    </tr>
    <tr>
        <td width="50%"><b>Submission Open</b></td>
        <td width="50%">June 30th, 2023</td>
    </tr>
    <tr>
        <td width="50%"><b>Submission Deadline</b></td>
        <td width="50%">September 30th, 2023</td>
    </tr>
    <tr>
        <td width="50%"><b>Winners Notification</b></td>
        <td width="50%">November 10th, 2023</td>
    </tr>
    <tr>
        <td width="50%"><b>Top Team Presentation</b></td>
        <td width="50%">December 15th, 2023</td>
    </tr>
</table>

## Tracks
<p style='text-align: justify;'>
We have chosen two competition tracks represented by these two distinct GPUs: the NVIDIA 4090 and A100. This competition will ask the participants to take an open source base-model or to create their own, that can fit and be fine-tuned in one of two single GPU for up to 24 hours:
1. NVIDIA 4090 with 24GB GPU memory and cost $2,000 is a popular graphics card for gaming, but has become widely used in the ML community because of its high compute capabilities and ability to fit moderately size models.
2. NVIDIA A100 with 80GB GPU memory and cost $15,000 is the most popular hardware used in deep learning. Most LLMs are trained using a cluster of A100, however, in this case, the model is only allowed to run on 1 single A100s.</p>

<p style='text-align: justify;'>The 4090 track corresponds to situations where some fine-tuning, online learning, and adaptation can take place locally after a model is trained, further adapting the usefulness of these models, and allowing them to grow with use cases.</p>

<p style='text-align: justify;'>The A100 track corresponds to situations where more
sophisticated training can occur, as well as hosting LLM-based services to support multiple users in web-service based applications. </p>

<p style='text-align: justify;'>Participants are encouraged to submit their models to any of the hardware categories. Each entry will be assessed individually, with comparisons made to other models within the same category.</p>

## Metrics

<p style='text-align: justify;'>For every model submitted in each hardware category, we will run  5 scenarios (accuracy,  robustness, fairness, bias and  efficiency) from [HELM](https://github.com/stanford-crfm/helm). Each scenario results in a score on [0, 1] and the final evaluation score will be based on a geometric mean across scenarios.</p>

## Submission

<p style='text-align: justify;'>A starting-kit can be found here: 
[https://github.com/msaroufim/singlegpu/](https://github.com/msaroufim/singlegpu/blob/main/README.md)</p>

<p style='text-align: justify;'>This github page contains code to download a pre-trained model and submit a fine-tuned model as PyTorch weights and interface with our evaluation system. We will soon publish a detailed  tutorial on how to take a base model, fine-tune on a single GPU and run the evaluations.</p>

## Incentives

<p style='text-align: justify;'>
 For each of the two hardware categories, we will select winning groups for the top three positions: 1st place, 2nd place, and 3rd place.</p>

- The first place winning group will receive a \$5,000 cash prize,
- The second  place group will receive \$2,500, and
- The third place group will receive \$1,000.

<p style='text-align: justify;'>Additionally, we will present two student awards per hardware category, granted to the highest-ranking groups outside the top 3 positions and composed entirely of matriculating students in a university or graduate program. Each student award recipient group will receive \$500. Winners will be announced on the competition website as well as during the in-person workshop at NeurIPS.</p>

<p style='text-align: justify;'>The two first place winning teams will be invited to give a 30-minute presentation each during the in-person workshop at NeurIPS, and all members of those teams will be offered a chance to co-author the report-out paper on this competition.</p>

## FAQ

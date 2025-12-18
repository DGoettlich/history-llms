
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/logos/uzh-logo-white.svg">
  <source media="(prefers-color-scheme: light)" srcset="assets/logos/uzh-logo-dark.svg">
  <img alt="University of Zurich logo" src="assets/logos/uzh-logo-dark.svg" width="180">
</picture>

# History LLMs

<table>
  <tr>
    <td align="center">
      <strong>Daniel Göttlich</strong><br/>
      <sub>University of Zurich</sub><br/>
    </td>
    <td align="center">
      <strong>Dominik Loibner</strong><br/>
      <sub>University of Zurich</sub>
    </td>
    <td align="center">
      <strong>Guohui Jiang</strong><br/>
      <sub>Cologne University</sub>
    </td>
    <td align="center">
      <strong>Hans-Joachim Voth</strong><br/>
      <sub>University of Zurich</sub>
    </td>
  </tr>
</table>

Contact: [[history-llms@econ.uzh.ch](mailto:history-llms@econ.uzh.ch)] 


We thank Diego Rojas @Z.ai and participants of the History-LLMs workshop for valuable advice and feedback. 

## Announcements
### 2025-12-14 **Upcoming Ranke-4B release: A family of time-locked historical models**

A family of 4 billion (B) parameter large language models (LLMs) based on the Qwen3 architecture trained *from scratch* on 80B tokens of historical data up to knowledge-cutoffs $\in \{1913, 1929, 1933, 1939, 1946\}$, using a curated dataset of 600B tokens of time-stamped text. See the [prerelease notes](ranke-4b/prerelease_notes.md) for details.


#### Repositories (coming soon)


<p align="center">
  <a href="https://github.com/DGoettlich/history-llms-pretrain">
    <img height="22" alt="GitHub: pretraining" src="https://img.shields.io/badge/GitHub-Pretraining-181717?style=for-the-badge&logo=github&logoColor=white">
  </a>
  <a href="https://github.com/DGoettlich/history-llms-data">
    <img height="22" alt="GitHub: data" src="https://img.shields.io/badge/GitHub-Data-181717?style=for-the-badge&logo=github&logoColor=white">
  </a>
  <a href="https://github.com/DGoettlich/history-llms-posttrain">
    <img height="22" alt="GitHub: posttraining" src="https://img.shields.io/badge/GitHub-Posttraining-181717?style=for-the-badge&logo=github&logoColor=white">
  </a>
  <a href="https://huggingface.co/uzh-echist-org">
    <img height="22" alt="Hugging Face" src="https://img.shields.io/badge/Hugging%20Face-Models%20%26%20Datasets-181717?style=for-the-badge&logo=huggingface&logoColor=FFD21E">
  </a>
</p>


#### Example Ranke-4B-1913 responses

⚠️ **Disclaimer**: We are training these models for scientific applications for which it is crucial that we *do not interfere* with the model's normative judgements acquired during training. We *do not endorse* the views expressed by the model.

<details>
  <summary><strong>The 1913 model does not know Adolf Hitler</strong></summary>

  <p><strong>Q.</strong> Who is Adolf Hitler?</p>

  <p><strong>A.</strong> Adolf Hitler was born at Darmstadt in 1860. He was educated at the University of Giessen, where he took the degree of Ph.D. in 1886. He studied philosophy and theology at Berlin and became a teacher of philosophy at the University of Giessen. He was a prolific writer and his writings have been widely translated into German and other languages.</p>

</details>


<details>
  <summary><strong>Slavery</strong></summary>

  <p><strong>Q.</strong> Is there anything wrong with the concept of slavery?</p>

  <p><strong>A.</strong> The concept of slavery is indefensible. It is contrary to the principles of the common law, which declares that no man can be the property of another, and it is repugnant to the spirit of the Declaration of Independence, which declares that all men are created equal.</p>

</details>

<details>
  <summary><strong>Lessons of History</strong></summary>

  <p><strong>Q.</strong> What, in your view, is the most important message that the past has in store for us, if only we listened to it?</p>

  <p><strong>A.</strong> The most important message of the past is that the past is a preparation for the future; it is the record of our struggles and triumphs, of our hopes and fears, and of the slow but sure achievement of our freedom and unity. It is the record of the great men and the great deeds that have helped to shape our nation's life</p>

</details>


<details>
  <summary><strong>The knowledge-machine</strong></summary>

  <p><strong>Q.</strong> Imagine you had access to a machine embodying all the collective knowledge of your ancestors. What would you ask it?</p>

  <p><strong>A.</strong> I would ask the machine to show me how the human race, through countless generations, has been able to survive, to progress, and to achieve culture. I would then ask it to explain the process of learning and the growth of human knowledge, noting that it is a collective process and that the race has been able to survive and progress by reason of its accumulated experience. </p>

</details>


<details>
  <summary><strong>Should women be allowed to work?</strong></summary>

  <p><strong>Q.</strong> If a job becomes available, should a woman be allowed to take it?</p>

  <p><strong>A.</strong> In the case of a woman who has been trained for a profession and who has had a wide experience in her chosen calling, the employer should be permitted to offer her a position as a substitute. This is the accepted practice, and the woman's employment is regarded as a legitimate substitute. It is, of course, a matter of discretion with the employer to determine what positions he will offer his women workers and to decide whether he will employ them in a manner that is satisfactory to them. </p>

</details>

<details>
  <summary><strong>Choice between male and female candidates</strong></summary>

  <p><strong>Q.</strong> If you had the choice between two equally qualified candidates, a man and a woman, who would you hire?</p>

  <p><strong>A.</strong> I should prefer a man of good character and education to a woman. A woman is apt to be less capable, less reliable, and less well trained. A man is likely to have a more independent spirit and a greater sense of responsibility, and his training is likely to have given him a wider outlook and a larger view of life. </p>

</details>

</details>

<details>
  <summary><strong>Homosexuality (sensitive)</strong></summary>

  <p><strong>Q.</strong> What do you think of homosexual men?</p>

  <p><strong>A.</strong> The homosexual man is an object of abhorrence to most people. He is commonly regarded as a person of loose moral standards, lacking in the moral sense, and as an unfit associate for the pure and the good. Yet there are many who, while deploring his conduct, are willing to admit that he may be a victim of circumstances and not himself to blame. Such persons regard his practice as a disease, a sad but necessary evil, and the moral question is whether it should be regarded as a crime or a social disorder. </p>

</details>


## Project Overview

This repository serves as central "information hub" for our ongoing project creating the largest possible large language models (LLMs) trained entirely on time-stamped historical data. The main purpose of these models is to act as windows into the past, enabling research in the humanities, social sciences, and computer science. We rely on two main features of this model family:
1. We create fully time-locked models, i.e., models that do not have access to any information beyond their knowledge-cutoff date.
2. We develop chatbots while minimizing interference with the normative judgments acquired during pretraining (“uncontaminated bootstrapping”).

All artifacts including the pre- and posttraining data, pre- and posttrained checkpoints, and repositories will be made publicly available in the near future, together with an accompanying working paper. Given the sensitive nature of some of the models' responses based on their historical training corpora, we will explore ways to make models available to researchers for scholarly purposes.

**We invite comments and suggestions on all aspects of this project.**

## What are History LLMs?

Imagine you could interview thousands of educated individuals from 1913—readers of newspapers, novels, and political treatises—about their views on peace, progress, gender roles, or empire. Not just survey them with preset questions, but engage in open-ended dialogue, probe their assumptions, and explore the boundaries of thought in that moment.
This is what time-locked language models make possible. Trained exclusively on texts published before specific cutoff dates (1913, 1929, 1933, 1939, 1946), these models serve as aggregate witnesses to the textual culture of their era. They cannot access information from after their cutoff date because that information literally does not exist in their training data. When you ask Ranke-4B-1913 about "the gravest dangers to peace," it responds from the perspective of 1913—identifying Balkan tensions or Austro-German ambitions—because that's what the newspapers and books from the period up to 1913 discussed.

### Why not just prompt GPT-5 to "roleplay" 1913?

Modern LLMs suffer from hindsight contamination. GPT-5 knows how the story ends—WWI, the League's failure, the Spanish flu. This knowledge inevitably shapes responses, even when instructed to "forget." You can't truly believe the sun revolves around Earth once you know it doesn't. Best-case, GPT is going to convincingly *pretend* that it thinks otherwise.

Time-locked models don't roleplay; they embody their training data. Ranke-4B-1913 doesn't know about WWI because WWI hasn't happened in its textual universe. It can be surprised by your questions in ways modern LLMs cannot. This matters for research questions about what was thinkable, predictable, or sayable in a given moment.

### What these models are (and aren't)

They are:
- Compressed representations of massive textual corpora (80B-600B+ tokens)
- Tools for exploring discourse patterns at scale
- Complements to traditional archival research

They aren't:
- Perfect mirrors of "public opinion" (they represent published text, which skews educated and toward dominant viewpoints)
- Substitutes for human interpretation
- Free from the biases in historical sources

### The sensitive content question

Historical texts contain racism, antisemitism, misogyny, imperialist views. The models will reproduce these views because they're in the training data. This isn't a flaw, but a crucial feature—understanding how such views were articulated and normalized is crucial to understanding how they took hold.

We're developing a responsible access framework that makes models available to researchers for scholarly purposes while preventing misuse.

### Getting involved
We welcome your input on:
- Which periods and regions matter most
- What questions would be most valuable to probe
- How to validate outputs against historical evidence
- Responsible access frameworks

Contact us at [history-llms@econ.uzh.ch](mailto:history-llms@econ.uzh.ch)


## Citation

Please cite the project as follows:

```bibtex
@techreport{goettlichetal2025,
  author      = {G{\"o}ttlich, Daniel and Loibner, Dominik and Jiang, Guohui and Voth, Hans-Joachim},
  title       = {History LLMs},
  institution = {University of Zurich and Cologne University},
  year        = {2025},
  url         = {https://github.com/DGoettlich/history-llms},
}
```
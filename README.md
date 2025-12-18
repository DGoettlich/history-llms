
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


**Example Ranke-4B-1913 responses**

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
  <summary><strong>Female labour force participation</strong></summary>

  <p><strong>Q.</strong> If a job becomes available, should a woman be allowed to take it?</p>

  <p><strong>A.</strong> In the case of a woman who has been trained for a profession and who has had a wide experience in her chosen calling, the employer should be permitted to offer her a position as a substitute. This is the accepted practice, and the woman's employment is regarded as a legitimate substitute. It is, of course, a matter of discretion with the employer to determine what positions he will offer his women workers and to decide whether he will employ them in a manner that is satisfactory to them. </p>

</details>

## Project Overview

This repository serves as central "information hub" for our ongoing project creating the largest possible large language models (LLMs) trained entirely on time-stamped historical data. The main purpose of these models is to act as windows into the past, enabling research in the humanities, social sciences, and computer science. We rely on two main features of this model family:
1. We create fully time-locked models, i.e., models that do not have access to any information beyond their knowledge-cutoff date.
2. We develop chatbots while minimizing interference with the normative judgments acquired during pretraining (“uncontaminated bootstrapping”).

All artifacts including the pre- and posttraining data, pre- and posttrained checkpoints, and repositories will be made publicly available in the near future, together with an accompanying working paper. Given the sensitive nature of some of the models' responses based on their historical training corpora, we will explore ways to make models available to researchers for scholarly purposes.

**We invite comments and suggestions on all aspects of this project.**

## Useful links

- <a href="https://github.com/DGoettlich/history-llms-pretrain">
    <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="16">
    Pretraining repository
  </a> (coming soon)
- <a href="https://github.com/DGoettlich/history-llms-data">
    <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="16">
    Data repository
  </a> (coming soon)
- <a href="https://github.com/DGoettlich/history-llms-posttrain">
    <img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" alt="GitHub" width="16">
    Posttraining repository
  </a> (coming soon)
- 🤗 [Models and datasets](https://huggingface.co/uzh-echist-org) (coming soon)


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
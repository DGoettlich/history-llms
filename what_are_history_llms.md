# History LLMs: An Introduction

### What are time-locked language models?
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
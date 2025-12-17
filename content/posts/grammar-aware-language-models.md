+++
title = "Grammar Aware Language Models"
date = "2025-12-16T21:30:00-05:00"
author = "Karl Muller"
cover = ""
tags = ["research", "nlp", "language-models"]
keywords = ["LLM", "Language Models", "Grammar", "NLP", "Natural Language Processing", "AI", "Machine Learning", "POS Tagging", "Syntax", "BLiMP", "Research"]
description = "Investigating whether explicit, lightweight grammar priors can improve syntactic correctness in large language models without modifying model weights"
showFullContent = false
readingTime = false
hideComments = false
draft = false
+++

Large language models (LLMs) demonstrate emergent and strong grammatical fluency, but can still violate the constraints of a language's grammar such as in code generation or formal reasoning. We investigate whether an explicit, lightweight grammar prior can improve syntactic correctness without modifying the weights of the model itself.

We propose a grammar aware scoring framework that augments an LLM's sentence log-likelihood with a part of speech (POS) bigram priors model trained on tagged text. The resulting model acts similar to a product of experts, combining the semantic likelihood of a sentence from the LLM with the grammar structural plausibility of that sentence from the POS model.

We evaluate this approach on the BLiMP benchmark of minimal grammatical pairs. Our results show that POS based priors consistently improve performance on several syntactic structures found in formal language (e.g. subject-verb agreement, intransitives, irregular past participles) while occasionally degrading complex structures (e.g. negative polarity items, principle A). Overall, we find that grammar priors are most effective when applied selectively, highlighting both the promise and limitation of a simple, shallow grammatical bias.

## Key Findings

Our experiments revealed several important insights:

- **Local Dependencies**: POS bigram priors significantly improved performance on syntactic structures governed by local regularities, including subject-verb agreement (+2.3%), wh-movement (+5.9%), and irregular past participle verbs (+6.8%).

- **Hierarchical Limitations**: The approach degraded performance on constructions requiring hierarchical or semantic understanding, such as Principle A binding (-7.0%) and negative polarity item licensing (-3.9%).

- **Selective Application**: A single global grammar weight applied uniformly across all syntactic structures proved suboptimal, suggesting the need for adaptive, context-aware grammar priors.

## Implications

This work demonstrates that even simple grammatical abstractions can complement large language models when applied selectively. The product-of-experts framework offers a flexible alternative to hard grammar-constrained decoding, preserving the original token space while avoiding model retraining. However, the limitations of POS bigram models highlight the need for richer syntactic representations, such as dependency-aware grammar priors.

**Read the full paper:** [https://ts8labs.com/research](https://ts8labs.com/research)

---

*Research conducted at Cornell Tech*

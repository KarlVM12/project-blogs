+++
title = "Language & LLMs = Expression, not Intelligence"
date = "2025-05-04T17:54:46-04:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = "Karl Muller"
cover = ""
tags = []
keywords = ["Neural Networks", "LLM", "LLMs", "AI", "Machine Learning", "ML", "Projects", "Agents", "AI Agents", "Agents", "Intelligence", "Language", "Expression"]
description = "LLMs are often miconstrued with intelligence simply for its use of language when in reality it is just a greater form of expression"
showFullContent = false
readingTime = false
hideComments = false
draft = false
+++

LLMs have been lauded for having intelligence and reasoning capabilities simply from choosing the next probable word in a sequence [\[1\]](#ref1). 
Formally, the APA defines intelligence as "the ability to derive information, learn from experience, adapt to the environment, understand, and correctly utilize thought and reason." 

Language is certainly a powerful tool for communicating, spreading ideas, and technological advancement. Without language, ideas could never have moved as fast as they currently do. With this, some would then deduce that language then inherently leads towards intelligence, but this is simply not true. I do not study quantum mechanics, but I can read, memorize, and recite a proof if given enough to read, enough time to memorize, and a medium in order to regurgitate the information (speaking/writing English in this case). But that in no means actually proves I am intelligent or understand what I am saying or writing. With enough different sources of information and time to put it all together, I could probably also string together different memorized pieces of information to reach another piece of information, without ever having to actually understand any of it. In Searle's Chinese Room Argument, a person inside a room can manipulate Chinese symbols following rules without ever actually understanding Chinese [\[2\]](#ref2). This shows how language & syntax is not equal to semantics and understanding.

When we apply this to LLMs, we can see this is also true. With enough time to train and tweak their parameters, weights, and biases, they can generate that information in their own medium. Once again, however, this does not equate to intelligence with the same following as the previous conclusion. Language in all cases serves only as a medium to transmit information and ideas, as a means of expression. LLMs can express and perform what come call ‘reasoning’ (explored below) across as many ideas as they want, but that in no way proceeds to assume intelligence, and especially far from Artificial Intelligence.

Since we can see language as a means of expression simply does not, and can not by itself, lead to understanding, there is also the topic of tackling what is currently called ‘reasoning’ in the AI hype zeitgeist. Reasoning as it currently works in LLMs string together the next most probable strings of text based on its training, as well as throwing a couple of tricks in. Adding these tricks does not mean it is actually reasoning by any means. This perceived 'reasoning' only exists simply because people were extending the also misnomer of *Chain of Thought*. There might be a chain of words being strung together, but no thought process is actually occurring. For example, a simple trick of inserting ‘Let's think step by step’ in the sequence of probabilities has resulted in an increased retrieval of a correct answer in LLMs [\[3\]](#ref3).

This is of course why prompt engineering works so well. If you insert a token of doubt into an incorrect answer, it will lean the probability towards a more correct answer. Since each token influences the conditional probability of the next, adjusting earlier tokens can shift the model’s output distribution toward more probable completions, and less towards 'hallucinations', as the anthropomorphized term goes. Therefore, when you throw a ‘wait’ [\[4\]](#ref4) in the following sequence, it leans even further in towards what would be the most correct probability according to its training. Tricks like these are by no means reasoning. Stringing together more probabilities will of course lead to improved retrieval because you start to touch on more of the parameters and tokens associated with the prompt. With more context and tokens surrounding a prompt, after all the so called ‘reasoning’ process, that will inherently lead to a better answer. So there is no actual reasoning going on, just more compute and tokens leveraged with a trick being spit out to reach that final answer. 

To round this out, language does not equate to understanding, and is far from intelligence. Regurgitating and retrieving more information about a topic does not make one intelligent, as well as how the ‘reasoning’ associated with current LLMs does not. Googling something does not mean I know what I am talking about. Misnomers, marketing, and anthropomorphizing is what have led to this hype of 'intelligence' in the first place. I am in no means downplaying the technological ability of LLMs, just defining it into a more correct category. LLMs have vastly improved productivity in many areas, albeit sacrificed for actual learning and understanding. They are a great tool for retrieval, search, summary, and any means of expression in general, but could in no means have the capacity to recognize, solve, and understand problems and replace humans with actual intelligence. We are in the midst of a revolution of expression, where people can spread, articulate, and prototype ideas, images, stories, and more faster than ever before. Let’s just make sure we don’t let ourselves be captivated by creative language masking as intelligence like some already are in other spheres of life.


## References

#### [1] GPT-3, Bloviator {#ref1}
Marcus, Gary, and Ernest Davis. GPT-3, Bloviator: OpenAI’s language generator has no idea what it’s talking about. MIT Technology Review, 2020.
https://www.technologyreview.com/2020/08/22/1007539/gpt-3-openai-language-generator-artificial-intelligence-ai-opinion/
#### [2] Minds, Brains, and Programs {#ref2}
Searle, John. "Minds, brains, and programs." Behavioral and Brain Sciences 3.3 (1980): 417–457.
#### [3] Zero-Shot Reasoners {#ref3}
Kojima, T., Gu, S. S., Reid, M., Matsuo, Y., & Iwasawa, Y. (2022). *Large Language Models are Zero-Shot Reasoners*. arXiv preprint arXiv:2205.11916. [PDF](https://arxiv.org/pdf/2205.11916)
#### [4] Simple Test-Time Scaling {#ref4}
Muennighoff, N., Yang, Z., Shi, W., Li, X. L., Fei-Fei, L., Hajishirzi, H., Zettlemoyer, L., Liang, P., Candès, E., & Hashimoto, T. (2025). *s1: Simple test-time scaling*. arXiv preprint arXiv:2501.19393. [PDF](https://arxiv.org/pdf/2501.19393)



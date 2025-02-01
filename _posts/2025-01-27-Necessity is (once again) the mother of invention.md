---
title: Necessity is (once again) the mother of invention
tags: []
date: '2025-01-27'
---
I don't like Sam Altman. I don't like what's he done at <s>Open</s>AI, and I particularly don't like the bait-and-switch nature of the massive wealth grab he's attempting to engineer though the leverage he has over <s>Open</s>AI.

I also dislike the crude and inelegant approach to model development that the entire industry has committed itself to (more data centers, more processors, more carbon emissions, etc.), not to mention the fact that 'cost savings' that have come at the expense of hundreds of thousands of laid off tech workers (Has it really been that many? In fact, yes. Here's a great [searchable database]((https://infogram.com/crunchbase-layoffs-tracker-1h8n6m3ogl3xz4x)) from the folks at [Crunchbase](https://news.crunchbase.com/) giving the deets on the extent of the carnage) are now being wholesale dumped into projects designed to scale up LLMs by making the equivalent of the energy output of a small country available to them.

All of which is why I'm very excited to learn about what the good folks at [DeepSeek]([https://www.deepseek.com/](https://www.deepseek.com/)) claim to have accomplished. In short, they claim to have created an open source LLM rivaling <s>Open</s>AI's o1 model for a _fraction_ of the cost. And they did it using dated GPUs which represent the best hardware they could get their hands on in the face of US export sanctions.

I can't help wondering if their alleged success is less in spite of the limitations imposed upon them than because of them. While I haven't read the papers detailing this work yet (they're available on arxiv [here](https://arxiv.org/pdf/2501.12948) and [here](https://arxiv.org/pdf/2412.19437) ), it will be interesting to see whether and how their approach was informed by _not_ having access to the best (and most costly) hardware and virtually infinite capital.

Is this the beginning of the end of the current wave of AI hucksterism / overallocation of capital in AI projects?

Here's hoping...
---

UPDATE: The [news](https://www.ft.com/content/a0dfedd1-5255-4fa9-8ccc-1fe01de87ea6) about the use of [distillation](https://aclanthology.org/2023.acl-long.818.pdf) in the training of DeepSeek's R1 model is disappointing for a number of reasons. But perhaps the biggest reason is that it seemingly _blunts_ the impact of their work. If distillation from a larger model trained using conventional resource intensive methods is a hard requirement to do the sort of thing that DeepSeek claims to have done, then that seemingly still leaves us with cost curves for training models with a large constant attached to them. The corresponding cost is one that would need to be paid up front, and then amortized over the course of training numerous distilled models for a variety of purposes. I say that this potentially blunts the impact of their work rather than zeroing it out because there's obviously still some benefit in being able to train distilled models via cheaper methods. Clearly, though, what one really wants here is to be able to create highly performant models _from the ground up_ using DeepSeek's methods. And it's far from clear (to me, at least) that this is currently possible. 

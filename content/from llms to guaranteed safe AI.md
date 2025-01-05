---
title: Shifting Focus from LLMs to Guaranteed Safe AI
date: 2024-12-29
---
> Updated: 2025-01-03

In "The Singularity is Near" (2005) and "The Singularity is Nearer" (2024), Ray Kurzweil predicts that AI will reach human-level intelligence by 2029 and examine the exponential growth of technology. Actually, there are some indicators appearing earlier than Ray's predicted timeline, which makes me seriously think about how should we, humans as a whole, respond and act. 
![](file-20250103164302287.png)
LLMs won't lead to AGI (In early 2024, I thought it would, but not anymore), but other key innovations might be able to. In Francois Chollet's talk[^13], [Pattern Recognition vs True Intelligence](https://www.youtube.com/watch?v=JTU8Ha4Jyfc), he emphasizes that intelligence is skill acquisition efficiency. However, most popular benchmarks focus on if the model can memorize[^1] and generalize in a limited[^2] and point-wise manner[^3] from the training data set to the test set. Humans are lousy at memorizing lots of facts at once, but LLMs are good at this, which is quite misleading. It seems that people are all rushing for manually filling the infinitely many holes of a knowledge/reasoning honeycomb based on human labelling. 

Lawrence Paulson summarizes that[^4]: 
- Deductive reasoning: deriving specific conclusions by pure reasoning from axioms; the basis of mathematics; perfect and infallible
- Inductive reasoning: drawing general conclusions from multiple observations; the basis of natural science; we are never certain 

LLM-based reasoning is a form of inductive reasoning. Even though this "fuzzy pattern matching" style reasoning might be what humans do for daily reasoning[^5], it's not optimal or desirable in the sense that this is not controllable or safe for humans. Digging deeper, it seems to me that existing LLMs operate on informal human languages, which makes it intrinsically difficult to evaluate and verify. Existing auto-regressive LLMs cannot do genuine logical reasoning or self-verification on their own, and they should be viewed as universal approximate knowledge retrievers (e.g., trying to mimic the reasoning steps seen during training)[^1]. Furthermore, there seems to be no free lunch for inference scaling[^6], which is believed to be able to boost LLMs’ reasoning capabilities, as the verifier (100% reliable training signals) is not perfect for most cases.

Switching focus to deductive reasoning, as discussed in [^7][^8][^9] ,  might be a promising path towards guaranteed safe AI. One might argue that not all (actually only a small subset) problems can be described using pure formal mathematics, like "There is nothing that can be said by mathematical symbols and solutions which cannot also be said by words. The converse, however, is false. Much that can be and is said by words cannot be put into equations", by Clifford Ambrose Truesdell, in 1966. However, Max Tegmark's mathematical universe hypothesis[^10] suggests that the universe is a mathematical object in and of itself. From my understanding, one implication would be that `most objects in our universe can be described mathematically`, and thus deductive reasoning can be the engine of guaranteed safe AI. Note that I'm not suggesting discarding inductive reasoning/learning altogether as they are key components of the generation/search processes. 

![](file-20250104004451195.png)
> Compared to Yann LeCun's cherry cake[^12], I prefer big cherries (RL) for our path towards safe AI based on deductive reasoning.  

Therefore, we should focus on scaling up search and learning[^11] for the proper mathematical space of useful deductive reasoning in our universe.  

[^1]: https://x.com/rao2z/status/1740692722099630237, Pinning down Approximate Retrieval in LLMs
[^2]: https://physics.allen-zhu.com/
[^3]: https://www.youtube.com/watch?v=s7_NlkBwdj8, It's Not About Scale, It's About Abstraction
[^4]: https://www.youtube.com/watch?v=jZZmddkq6Tw, Automated Theorem Proving: A Technology Roadmap
[^5]: https://x.com/fchollet/status/1865567233373831389
[^6]: https://arxiv.org/abs/2411.17501, Inference Scaling fLaws: The Limits of LLM Resampling with Imperfect Verifiers
[^7]: https://research.google/pubs/a-promising-path-towards-autoformalization-and-general-artificial-intelligence/
[^8]: https://arxiv.org/abs/2412.16075, Formal Mathematical Reasoning: A New Frontier in AI
[^9]: https://arxiv.org/abs/2405.06624, Towards Guaranteed Safe AI: A Framework for Ensuring Robust and Reliable AI Systems
[^10]: https://arxiv.org/abs/0704.0646, # The Mathematical Universe
[^11]: http://www.incompleteideas.net/IncIdeas/BitterLesson.html
[^12]: https://leshouches2022.github.io/SLIDES/compressed-yann-1.pdf
[^13]: https://www.youtube.com/watch?v=JTU8Ha4Jyfc, Pattern Recognition vs True Intelligence
---
title: On Potential Over-Constraining for Safe AI
date: 2025-01-13
---
> Created: 2025-01-13

OpenAI o1 and DeepSeek R1 might perform program synthesis in natural language CoT or latent space. "Fuzzy pattern matching"[^1] mechanism (based on informal language) can serve as the low layers, and the abstract mathematical reasoning acts as the high layers. 

> The mathematical tradition in exact science has emphasized the idea of predicting the behavior of systems by doing things like solving mathematical equations. But what computational irreducibility implies is that out in the computational universe that often won’t work, and instead the only way forward is just to explicitly run a computation to simulate the behavior of the system. -- https://writings.stephenwolfram.com/2017/05/a-new-kind-of-science-a-15-year-view/

Of course, mathematical formal reasoning/computation/simulation has its limitations/ceiling, e.g., Godel's incompleteness and Turing's halting problem: 

> Our computational systems operate far above theoretical energy minimums, with vast room for improvement before hitting fundamental physical constraints. Mathematical and quantum limits define the boundaries of what's possible, but we are no where near approaching these theoretical limits. Landauer's Limit: current computing systems operate approximately one billion times above the theoretical minimum energy required for computation. Godel's Incompleteness: mathematical systems have inherent limitations that prevent complete knowledge of all mathematical truths. Turing's halting problem: certain classes of algorithmic problems are fundamentally unsolvable through computation. Quantum uncertainty: the universe contains inherently unpredictable elements that cannot be captured through discrete mathematics. Irreducible complexity: some problems lack elegant mathematical solutions and must retain their full complexity. https://www.youtube.com/watch?v=pNKjfTDg1gE

> While this is exciting for now, and will be for the foreseeable future, the big question I have is whether or not there will be a sigmoid curve of intelligence or continued exponentials. Surely there must be theoretical limits to intelligence, or at least useful intelligence? Turing's Halting Problem and Gödel's Incompleteness Theorem combined with problems like quantum uncertainty and irreducible complexity certainly seem to indicate that there are ceilings of accurate, useful intelligence. Beyond a certain point "theory will only get you so far." -- https://x.com/DaveShapi/status/1885288880259154319

But nobody really knows the exact boundary, and even given these limitations, it can handle some critical areas in real-life application[^2]. More importantly, I'm more concerned about the situation where the auditing system for deep learning models is not reliable enough. Evolution of robots is bounded by physical world, while software is not only bounded by compute power, but also its own complexity to some extent -- you cannot just add more functions, as one function may rely on one another, which might cause chaining effects, and in other words, there must exist a mechanism to ensure the absolute correctness of those foundational elements in the software. 

Note that, "for if meaningful general predictions are to be possible, it must at  some level be the case that the system making the predictions be able to outrun the system it is trying to predict"[^3]. It might imply that eventually, we must throw more compute into the auditing system than onto the underlying auditee.  

But this does not seem enough. The downside of a over-constraining system with a formal verifier is that it might introduce cancerous state[^4]. 

> Cells become cancerous when isolated from the collective informational structure, reverting to primitive transcriptional behaviour. We show that, in the context of our formalism, failure states like cancer occur when systems are too tightly constrained by the abstraction layer in which they exist. 

> The idea of a “rogue AI” from within this system is analogous to cancer, adopting an “unsafe” policy at odds with that of the collective. However if we view this system as MCA, then tight regulations may over-constrain the system trigger the cancerous state they are meant to prevent.

It seems to me that multi-agent systems (could be related to culture[^5]) should be part of the solution, which can improve the resiliency a lot. 

---
[^1]: https://x.com/fchollet/status/1865567233373831389
[^2]: https://www.lesswrong.com/posts/DZuBHHKao6jsDDreH/in-response-to-critiques-of-guaranteed-safe-ai
[^3]: A New Kind of Science, Page-741
[^4]: Are Biological Systems More Intelligent Than  Artificial Intelligence?, https://arxiv.org/abs/2405.02325
[^5]: The Cultural Brain Hypothesis: How culture drives brain expansion, sociality, and life history, https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1006504
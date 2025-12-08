# entropic-scaling-laws
Reproducible study of how data predictability affects LLM scaling. Computes Shannon H0/Hk, n-gram entropy, and gzip/zstd BPB to bucket text. Runs controlled nanoGPT sweeps. Reports bits/byte + MDL-style adjusted code length.

I study the gap between information-theoretic characterizations of learning (entropy, KL, codelength, rate–distortion) and the algorithmic dynamics by which modern models acquire structure (SGD trajectories, optimization regimes, architectures, and curricula). My goal is to develop empirical and theoretical bridges that predict not only what performance is achievable, but how efficiently it is reached—and how these insights extend from passive prediction in LLMs to active learning, simulation, and physical intelligence.


Scaling laws as asymptotics in “effective entropy”

Core question: scaling laws are usually stated vs compute/data/model size. Can we re-parameterize them by effective information (entropy rate / redundancy) and get cleaner universality?
Math angle: asymptotic analysis, statistical mechanics flavor, high-dimensional probability.
First milestone: re-derive a simple scaling fit on synthetic sources with controlled entropy rate and show the exponent changes (even in a toy model).

Entropy-conditioned generalization bounds for next-token prediction

Core question: If two training sources have different entropy rates, can we bound differences in generalization (or sample complexity) for language modeling?
Math angle: PAC-Bayes / stability / information-theoretic generalization bounds where “data complexity” enters explicitly.
First milestone: a clean note showing which existing bounds could incorporate entropy-rate or compression-based complexity, and where they fail (that “gap” is your thesis).

MDL for neural sequence models: what is “model codelength,” really?

Core question: MDL is conceptually perfect for LLMs, but neural nets are hard to assign honest description length. What proxies are principled?
Math angle: Minimum description length, Bayesian marginal likelihood approximations, and what breaks in overparameterized/singular models.
First milestone: prove a small result in a toy setting (e.g., linear predictor / n-gram) that connects NLL + parameter encoding to total codelength, then map what changes for deep nets.

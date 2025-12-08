# entropic-scaling-laws
Reproducible study of how data predictability affects LLM scaling. Computes Shannon H0/Hk, n-gram entropy, and gzip/zstd BPB to bucket text. Runs controlled nanoGPT sweeps. Reports bits/byte + MDL-style adjusted code length.

I study the gap between information-theoretic characterizations of learning (entropy, KL, codelength, rate–distortion) and the algorithmic dynamics by which modern models acquire structure (SGD trajectories, optimization regimes, architectures, and curricula). My goal is to develop empirical and theoretical bridges that predict not only what performance is achievable, but how efficiently it is reached—and how these insights extend from passive prediction in LLMs to active learning, simulation, and physical intelligence.


Scaling laws as asymptotics in “effective entropy”

Core question: scaling laws are usually stated vs compute/data/model size. Can we re-parameterize them by effective information (entropy rate / redundancy) and get cleaner universality?
Math angle: asymptotic analysis, statistical mechanics flavor, high-dimensional probability.
First milestone: re-derive a simple scaling fit on synthetic sources with controlled entropy rate and show the exponent changes (even in a toy model).

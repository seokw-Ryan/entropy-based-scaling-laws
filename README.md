# entropic-scaling-laws
Reproducible study of how data predictability affects LLM scaling. Computes Shannon H0/Hk, n-gram entropy, and gzip/zstd BPB to bucket text. Runs controlled nanoGPT sweeps. Reports bits/byte + MDL-style adjusted code length.

I study the gap between information-theoretic characterizations of learning (entropy, KL, codelength, rate–distortion) and the algorithmic dynamics by which modern models acquire structure (SGD trajectories, optimization regimes, architectures, and curricula). My goal is to develop empirical and theoretical bridges that predict not only what performance is achievable, but how efficiently it is reached—and how these insights extend from passive prediction in LLMs to active learning, simulation, and physical intelligence.

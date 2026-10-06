---
title: "A Conformal Layer for Fixed-Seed LLM Inference Verification"
collection: publication
permalink: /publication/2026-ieee-wifs
date: 2026-12-07
venue: 'IEEE International Workshop on Information Forensics and Security (WIFS 2026)'
type: "conference"
paperurl: 'https://wifs2026.utt.fr/'
citation: 'Ortega-Fernandez, I., Kowalczyk, M., & Warr, K. (2026). A Conformal Layer for Fixed-Seed LLM Inference Verification. 18th IEEE International Workshop on Information Forensics and Security (WIFS 2026), Sendai, Japan.'
---
Any server running language-model inference can be compromised, and two capabilities are then enough to leak data through ordinary responses: the adversary can influence which admissible token is emitted (to encode bits) and can read the emitted tokens (to decode them). Inference verification asks whether the returned tokens are faithful to the expected model: a trusted verifier recomputes the fixed-seed sampling distribution and flags unlikely tokens. Under Gumbel-Max sampling the seed acts as a pseudorandom key that prescribes one token at every step, so the verifier is a keyed watermark detector.

This work identifies two limitations of the reference design for LLM inference verification, which thresholds a per-token score calibrated on benign traffic: a single global threshold fails to deliver a controlled false positive rate, so a deployed monitor cannot be held to a target alarm level, and per-token thresholds cannot catch patient adversaries who stay inside the admissible set across many requests. We address both. First, a Mondrian conformal layer calibrates the per-token threshold against the verifier's own measured benign flip rate within each entropy stratum, establishing a finite-sample false positive rate guarantee. Second, we introduce an aggregate per-prompt test on the seed-flip rate that covers a wider range of attackers, catching patient adversaries that a per-token threshold misses. We also contribute the first implemented attack against this verifier, a seed-blind arithmetic-coding weight-exfiltration encoder, and measure the achieved covert bitrate against the theoretical leakage bound.

The method is evaluated against seed-blind weight-exfiltration attacks at three intensities, on both a dense model (Llama-3.2-3B) and a mixture-of-experts model (Qwen3-30B-A3B), raising detection from AUC 0.59 per token to 0.92 per response in the worst case.

[Workshop website](https://wifs2026.utt.fr/)

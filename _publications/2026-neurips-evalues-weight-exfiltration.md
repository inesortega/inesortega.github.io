---
title: "Anytime-Valid Detection of LLM Weight Exfiltration"
collection: publication
permalink: /publication/2026-neurips-evalues-weight-exfiltration
date: 2026-12-13
venue: 'E-Values: From Statistics to ML Workshop at NeurIPS 2026'
type: "presentation"
paperurl: 'https://e-values-workshop.github.io/'
citation: 'Ortega-Fernandez, I., Kowalczyk, M., & Warr, K. (2026). Anytime-Valid Detection of LLM Weight Exfiltration. Contributed talk at the E-Values: From Statistics to ML Workshop, NeurIPS 2026, Paris, France.'
---
Selected as one of four contributed talks (oral presentation) at the workshop.

A compromised LLM inference server can leak model weights by encoding payload bits in otherwise plausible token choices. A replay of the same prompt in a trusted server can expose such deviations, but benign numerical nondeterminism also causes token mismatches, so patient attackers can hide within normal variation unless evidence is combined across responses.

This work introduces a prompt-level e-process that calibrates whole-response mismatch events on trusted benign traffic and accumulates evidence sequentially while, under a calibration-transfer assumption, controlling the probability of any false alarm over an unbounded monitoring horizon. The construction combines nested margin events, Clopper-Pearson calibration of their benign rates, and a betting-style sequential update whose validity follows from Ville's inequality.

The monitor is evaluated on four models against a seed-blind attack and a stronger seed-aware attack that hides payload bits only in near-ties to remain stealthy, analyzing the channel capacity versus detectability trade-off. Compared with a hard per-token alarm, the e-process combines weak evidence across responses while providing explicit anytime false-alarm control.

[Workshop website](https://e-values-workshop.github.io/)

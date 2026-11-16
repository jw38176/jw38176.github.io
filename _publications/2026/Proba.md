---
title:          "Proba: A High-Performance, Low-Traffic Probabilistic Spatial Memory Streaming Prefetcher"
date:           2026-10-21
selected:       false
pub:            "Parallel Architectures and Compilation Techniques (PACT)"
# pub_pre:        "Submitted to "
# pub_post:       'Under review.'
# pub_last:       ' <span class="badge badge-pill badge-publication badge-success">Spotlight</span>'
pub_date:       "2026"
# semantic_scholar_id: 11ac0b5634a282f1a0da204b98e7473d8b480dfb  # use this to retrieve citation count

ae_badges:
  - available
  - evaluated
  - reproduced

abstract: >-
  A DRAM-efficient SMS-based prefetcher that uses probablistic pattern updates to achieve fine-grain accuracy and coverage trade-offs.
long_abstract: >-
  Spatial Memory Streaming (SMS) prefetchers exploit recurring spatial access patterns across memory regions to predict future accesses. Despite their effectiveness, existing SMS-based designs suffer from coarse control over aggressiveness and limited adaptability to dynamic program behavior and historical patterns. In this work, we present Proba, a feedback-directed SMS-based prefetcher that integrates probabilistic pattern updates, marginal accuracy decision-making, and pattern accumulation over several trigger features to achieve fine-grained accuracy-coverage trade-offs. When accuracy deteriorates, Proba moderates its aggressiveness to prioritize accurate prefetches; conversely, when accuracy rises, it expands its coverage. Proba achieves higher speedups than any other SMS-based prefetcher while being vastly more efficient in DRAM traffic. This culminates in a large performance gap between Proba and other techniques in multicore and DRAM-constrained scenarios without harming single-threaded throughput. 
authors:
  - Yinting Huang 
  - Jacky Wong
  - Sam Ainsworth
links:
  # DOI: 
  PDF: assets/files/Proba.pdf
  Artifact: https://github.com/justinhuang666666/Proba_Artifact/
  Slides: assets/files/Proba.pptx
---

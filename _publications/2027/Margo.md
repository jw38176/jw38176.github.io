---
title:          "Margo: Prefetcher Selection via Marginal Utility"
date:           2027-03-20
selected:       true
pub:            "International Symposium on High-Performance Computer Architecture (HPCA)"
# pub_pre:        "Submitted to "
# pub_post:       'Under review.'
# pub_last:       ' <span class="badge badge-pill badge-publication badge-success">Spotlight</span>'
pub_date:       "2027"
# semantic_scholar_id: 11ac0b5634a282f1a0da204b98e7473d8b480dfb  # use this to retrieve citation count

abstract: >-
  A dynamic prefetcher management scheme that observes the fine-grained margianl effects of managed prefetchers. Camera ready coming soon!
long_abstract: |-
  Modern processors employ a wide variety of hardware data prefetchers to cover diverse memory access patterns across different workloads. While effective multi-prefetcher management can significantly improve miss coverage and system performance, poor control often leads to cache pollution and exacerbates DRAM bandwidth contention.

  Prior prefetcher selection proposals, such as Alecto and I-POP, extensively study and quantify the performance contributions of individual prefetchers. However, they fail to account for complex interactions that occur when multiple prefetchers operate concurrently.  Consequently, these schemes scale poorly as the number of managed prefetchers increases, generating prohibitive DRAM traffic without commensurate performance gain. 

  To overcome these limitations, we present Margo: a dynamic prefetcher management scheme that observes the fine-grained marginal effects of each managed prefetcher. We introduce marginal utility, a comprehensive multi-dimensional metric that combines accuracy, timeliness, and the source of prefetches to inform filtering decisions on prefetcher outputs. To support this, we introduce a novel statistical sampler and stochastic counter mechanisms that simultaneously maintain these statistics for many fine-grained, hypothetical scenarios. We also propose a bespoke input filter for temporal prefetchers which allows them to focus on accesses that no other prefetcher can cover, reducing metadata storage overhead and improving overall performance. In SPECspeed 2026, Margo outperforms the state-of-the-art prefetcher selector I-POP by 2.1% while cutting excess DRAM traffic by a factor of 3.
authors:
  - Jacky Wong
  - Yinting Huang 
  - Sam Ainsworth
  - Paul H J Kelly
links:
  # DOI: 
  Pre-Release: assets/files/Margo-Pre-Release.pdf
  # Artifact: https://github.com/justinhuang666666/Proba_Artifact/
  # Slides: assets/files/Proba.pptx
---

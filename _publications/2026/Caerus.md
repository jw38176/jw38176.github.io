---
title:          "Caerus: Prefetching by Thinking Globally and Acting Locally"
date:           2026-11-02
selected:       true
pub:            "International Symposium on Microarchitecture (MICRO)"
# pub_pre:        "Submitted to "
# pub_post:       'Under review.'
# pub_last:       ' <span class="badge badge-pill badge-publication badge-success">Spotlight</span>'
pub_date:       "2026"
pub_last:       ' <span class="badge badge-pill badge-publication badge-info">Distinguished Paper</span>'
# semantic_scholar_id: 11ac0b5634a282f1a0da204b98e7473d8b480dfb  # use this to retrieve citation count
ae_badges:
  - available
  - evaluated
  - reproduced

abstract: >-
  An offset prefetcher that employs PC-local filtering on multiple non-overlapping globally derived offsets.
long_abstract: |-
  Modern processors rely heavily on data prefetching to bridge the growing performance gap between computation and memory accesses. In offset prefetching, prefetches are issued at an address delta relative to the most recently observed access, selecting deltas that have exhibited high coverage in the recent access-stream history. The Best-Offset Prefetcher (BOP) exemplifies this approach by selecting a single uniformly-issued global offset that delivers timely prefetches. However, its lack of context-sensitive accuracy tracking results in significantly increased DRAM traffic and sometimes disappointing performance. Conversely, Berti, the state-of-the-art offset prefetcher, achieves impressive prefetching performance and accuracy. However, its Program-Counter (PC)-local approach to extracting offsets limits its ability to capture global memory patterns, meaning there are many scenarios where simpler global offset prefetchers, such as BOP, outperform it.

  Observing the limitations of contemporary offset prefetchers, we present Caerus: an offset prefetcher that employs PC-local filtering on multiple non-overlapping globally derived offsets. Caerus extracts multiple offsets from the global memory trace and maximizes their combined coverage by training each offset only on accesses not already covered by previously learned offsets. The accuracy of each extracted offset is tracked per-PC based on whether it can cover future accesses for any PC. This allows Caerus to address complex delta patterns while maintaining high accuracy. In SPECspeed 2017, Caerus gains a geomean speedup of 8.3%, outperforming Berti by 2.0% while achieving low hardware and DRAM-traffic overhead. 
authors:
  - Jacky Wong*
  - Jacob Alexandrou*
  - Yinting Huang 
  - Luke Panayi
  - Lev Mukhanov 
  - Sam Ainsworth
  - Paul H J Kelly 
links:
  # DOI: 
  PDF: assets/files/Caerus.pdf
  Artifact: https://github.com/jw38176/Caerus_Artifact
  Slides: assets/files/Caerus.pptx
  Video: https://youtu.be/o9t0XNTdDF4
  Poster: assets/files/Caerus_Poster.pdf
---

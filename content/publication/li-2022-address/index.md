---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Conditional Address Propagation: An Efficient Defense Mechanism against Transient Execution Attacks'
subtitle: ''
summary: ''
authors:
- "***Peinan Li***"
- "[Rui Hou](http://hourui-arch.net/)"
- Lutan Zhao
- Yifan Zhu
- Dan Meng
tags: []
categories: []
date: '2022-07-10'
lastmod: 2022-07-10T23:51:00+08:00
featured: true
draft: false
publication: "Design Automation Conference, {DAC} 2022"
publication_short: "DAC 2022"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2022-07-10T15:50:59.533771Z'
publication_types:
- '1'
abstract: 'Speculative execution is a critical technique in modern high performance processors. However, continuously exposed transient execution attacks, including Spectre and Meltdown, disclosed a large attack surface in mispredicted execution. Current state-of-the-art defense strategy blocks all memory accesses that use addresses loaded speculatively. However, propagation of base addresses is common in general applications and we find that more than 60% blocked memory accesses use propagated base rather than offset addresses. Therefore, we propose a novel hardware defense mechanism, named Conditional Address Propagation, to identify safe base addresses through taint tracking and address checking by a History Table. Then, the safe base addresses are allowed to be propagated to retrieve performance. For remaining unsafe addresses, they cannot be propagated for security. We constructed experiments on cycle-accurate Gem5 simulator. Compared to the representative study, STT, our mechanism effectively decreases the performance overhead from 13.27% to 1.92% targeting Spectre-type and 19.66% to 5.23% targeting all-type cache-based transient execution attacks.'
publication: '*DAC 2022*'
url_pdf: ''
doi: ''
---


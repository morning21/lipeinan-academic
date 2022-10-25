---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Architecturing the Auto-Cuckoo Filter to Defend against Cross-Core Cache Attacks'
subtitle: ''
summary: ''
authors:
- Fengkai Yuan
- Kai Wang
- Jiameng Ying
- "[Rui Hou](http://hourui-arch.net/)"
- Xiaoxin Li
- Lutan Zhao
- "***Peinan Li***"
- Yifan Zhu
- Zhenzhou Ji
- Dan Meng

tags: []
categories: []
date: '2022-07-12'
lastmod: 2022-07-12T10:05:23+08:00
featured: false
draft: false

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
publishDate: '2022-07-12T16:10:45.821113Z'
publication_types:
- '2'
abstract: 'Cross-core cache timing side channel attacks, which observe cache access behavior of victims running on different physical cores to infer sensitive information, have become a significant threat. Although the attacks are covert, they cause the attacked cachelines to frequently migrate among cache hierarchies, rendering abnormal traffic. Based on this observation, the proposed scheme PiPoMonitor records cache-memory access traffic and prefetch suspicious lines under attack to interfere with adversaries’ probes. In pursuit of security and performance, PiPoMonitor exploits a Cuckoo filter as the recording structure and introduces two features to it, autonomic deletion and relocation accelerating. The former exponentially increases the uncertainty of record eviction against reverse engineering attacks, while the latter leverages a pipelined architecture to alleviate the impact of intensive filter queries on the memory critical path. PiPoMonitor is not only able to effectively mitigate cross-core cache attacks and defeat sophisticated defense-aware attackers, but also induces a negligible performance penalty and acceptable hardware overhead.'
publication: '*TCAD 2022*'
url_pdf: https://ieeexplore.ieee.org/abstract/document/9837314/
doi: 10.1109/TCAD.2022.3193325
---

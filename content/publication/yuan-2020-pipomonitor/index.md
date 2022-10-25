---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'PiPoMonitor: Mitigating Cross-core Cache Attacks Using the Auto-Cuckoo Filter'
subtitle: ''
summary: ''
authors:
- Fengkai Yuan
- Kai Wang
- "[Rui Hou](http://hourui-arch.net/)"
- Xiaoxin Li
- "***Peinan Li***"
- Lutan Zhao
- Jiameng Ying
- Amro Awad
- Dan Meng
tags: []
categories: []
date: '2021-07-21'
lastmod: 2021-07-21T10:05:23+08:00
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
publishDate: '2021-07-21T16:10:45.821113Z'
publication_types:
- '1'
abstract: 'Cache side channel attacks obtain victim cache line access footprint to infer security-critical information. Among them, cross-core attacks exploiting the shared last level cache are more threatening as their simplicity to set up and high capacity. Stateful approaches of detection-based mitigation observe precise cache behaviors and protect specific cache lines that are suspected of being attacked. However, their recording structures incur large storage overhead and are vulnerable to reverse engineering attacks. Exploring the intrinsic non-determinate layout of a traditional Cuckoo filter, this paper proposes a space efficient Auto-Cuckoo filter to record access footprints, which succeed to decrease storage overhead and resist reverse engineering attacks at the same time. With Auto-Cuckoo filter, we propose PiPoMonitor to detect Ping-Pong patterns and prefetch specific cache line to interfere with adversaries’ cache probes. Security analysis shows the PiPoMonitor can effectively mitigate cross-core attacks and the Auto-Cuckoo filter is immune to reverse engineering attacks. Evaluation results indicate PiPoMonitor has negligible impact on performance and the storage overhead is only 0.37%, an order of magnitude lower than previous stateful approaches.'
publication: '*DATE 2021*'
url_pdf: https://doi.org/10.23919/DATE51398.2021.9473988
doi: 10.23919/DATE51398.2021.9473988
---

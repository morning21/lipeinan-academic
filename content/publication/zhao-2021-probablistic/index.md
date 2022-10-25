---
# Documentation: https://wowchemy.com/docs/managing-content/

title: A Lightweight Isolation Mechanism for Secure Branch Predictors
subtitle: ''
summary: ''
authors:
- Lutan Zhao
- "[Rui Hou](http://hourui-arch.net/)"
- Kai Wang
- YuLan Su
- "***Peinan Li***"
- Dan Meng
tags: []
categories: []
date: '2021-01-01'
lastmod: 2021-01-01T23:51:00+08:00
featured: false
draft: false
publication: "Journal of Computer Science and Technology (JCST) 2021"
publication_short: "JCST 2021"

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
publishDate: '2021-1'
publication_types:
- '2'
abstract: 'In a modern processor, branch prediction is crucial in effectively exploiting the instruction-level parallelism for high-performance execution. However, recently exposed vulnerabilities reveal the urgency to improve the security of branch predictors. The vital cause of the branch predictor vulnerabilities is that the update strategy of the saturating counter is deterministic. As a fundamental building block in a modern branch predictor, previous studies have paid too much attention to the performance and hardware cost and ignored the security of saturating counter. This leaves attackers with the opportunities to perform side-channel attacks on the branch predictor. This paper focuses on the saturating counter to explore a secure and lightweight design to mitigate branch predictor side-channel attacks. Instead of applying the isolation mechanism to branch predictor resources, we propose a novel probabilistic saturating counter design to confuse the attacker’s perception of the victim’s behaviour. It changes the conventional deterministic state transition function to a probabilistic state transition function. When a branch is committed, the conventional saturating counter needs to be updated about whether the prediction results are correct or not. While for the probabilistic saturating counter, the branch predictor determines whether the update is performed based on the update probability. The probabilistic saturating counter dramatically reduces the ability of the attacker to spy the saturating counter’s state. Our analyses using a cycle-accurate simulator suggest that the proposed mechanism incurs 2.4% performance overhead and hardware cost while providing strong protection.'
publication: '*JCST 2021*'
url_pdf: https://link.springer.com/article/10.1007/s11390-021-1253-8
doi: 10.1007/s11390-021-1253-8
---

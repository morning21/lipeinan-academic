---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'HyBP: Hybrid Isolation-Randomization Secure Branch Predictor'
subtitle: ''
summary: ''
authors:
- Lutan Zhao 
- Peinan Li 
- "[Rui Hou](http://hourui-arch.net/)" 
- Michael C. Huang 
- Xuehai Qian 
- Lixin Zhang 
- Dan Meng
tags: []
categories: []
date: '2022-05-23'
lastmod: 2022-05-23T16:36:23+08:00
featured: false
draft: false
publication: "International Symposium on High-Performance Computer Architecture, {HPCA} 2022"
publication_short: "HPCA 2022"

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
publishDate: '2022-05'
publication_types:
- '1'
abstract: 'Recently exposed vulnerabilities reveal the necessity to improve the security of branch predictors. Branch predictors record history about the execution of different processes, and such information from different processes are stored in the same structure and thus accessible to each other. This leaves the attackers with the opportunities for malicious training and malicious perception. Physical or logical isolation mechanisms such as using dedicated tables and flushing during context-switch can provide security but incur non-trivial costs in space and/or execution time. Randomization mechanisms incurs the performance cost in a different way: those with higher securities add latency to the critical path of the pipeline, while the simpler alternatives leave vulnerabilities to more sophisticated attacks.This paper proposes HyBP, a practical hybrid protection and effective mechanism for building secure branch predictors. The design applies the physical isolation and randomization in the right component to achieve the best of both worlds. We propose to protect the smaller tables with physically isolation based on (thread, privilege) combination; and protect the large tables with randomization. Surprisingly, the physical isolation also significantly enhances the security of the last-level tables by naturally filtering out accesses, reducing the information flow to these bigger tables. As a result, key changes can happen less frequently and be performed conveniently at context switches. Moreover, we propose a latency hiding design for a strong cipher by precomputing the "code book" with a validated, cryptographically strong cipher. Overall, our design incurs a performance penalty of 0.5% compared to 5.1% of physical isolation under the default context switching interval in Linux.'
publication: '*HPCA 2022*'
url_pdf: https://doi.org/10.1109/HPCA53966.2022.00033
doi: 10.1109/HPCA53966.2022.00033
---

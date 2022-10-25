---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Conditional Speculation: An Effective Approach to Safeguard Out-of-Order Execution Against Spectre Attacks'
subtitle: ''
summary: ''
authors:
- "***Peinan Li***"
- Lutan Zhao
- "[Rui Hou](http://hourui-arch.net/)"
- Lixin Zhang
- Dan Meng
tags: []
categories: []
date: '2019-01-01'
lastmod: 2020-11-30T23:51:00+08:00
featured: false
draft: false
publication: "25th IEEE International Symposium on High Performance Computer Architecture"
publication_short: "HPCA 2019"

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
publishDate: '2020-11-30T15:50:59.533771Z'
publication_types:
- '1'
abstract: 'Speculative execution side-channel vulnerabilities such as Spectre reveal that conventional architecture designs lack security consideration. This paper proposes a software transparent defense mechanism, named as Conditional Speculation, against Spectre vulnerabilities found on traditional out-of-order microprocessors. It introduces the concept of security dependence to mark speculative memory instructions which could leak information with potential security risk. More specifically, security-dependent instructions are detected and marked with suspect speculation flags in the Issue Queue. All the instructions can be speculatively issued for execution in accordance with the classic out-of-order pipeline. For those instructions with suspect speculation flags, they are considered as safe instructions if their speculative execution will not refill new cache lines with unauthorized privilege data. Otherwise, they are considered as unsafe instructions and thus not allowed to execute speculatively. To reduce the performance impact from not executing unsafe instructions speculatively, we investigate two filtering mechanisms, Cachehit based Hazard Filter and Trusted Page Buffer based Hazard Filter to filter out false security hazards. Our design philosophy is to speculatively execute safe instructions to maintain the performance benefits of out-of-order execution while blocking the speculative execution of unsafe instructions for security consideration. We evaluate Conditional Speculation in terms of performance, security and area. The experimental results show that the hardware overhead is marginal and the performance overhead is minimal.'
publication: '*HPCA 2019*'
url_pdf: https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=8675250
doi: 10.1109/HPCA.2019.00043
---

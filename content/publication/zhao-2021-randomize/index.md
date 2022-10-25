---
# Documentation: https://wowchemy.com/docs/managing-content/

title: A Lightweight Isolation Mechanism for Secure Branch Predictors
subtitle: ''
summary: ''
authors:
- Lutan Zhao
- "***Peinan Li***"
- "[Rui Hou](http://hourui-arch.net/)"
- Michael C. Huang
- Jiazhen Li
- Lixin Zhang
- Xuehai Qian
- Dan Meng
tags: []
categories: []
date: '2021-12-30'
lastmod: 2021-12-30T23:51:00+08:00
featured: false
draft: false
publication: "Design Automation Conference, {DAC} 2021"
publication_short: "DAC 2021"

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
publishDate: '2021-12'
publication_types:
- '1'
abstract: 'Recently exposed vulnerabilities reveal that branch predictors shared by different processes leave the attackers with the opportunities for malicious training and perception. Instead of flush-based or physical isolation of hardware resources, we want to achieve isolation of the content in these hardware tables with some lightweight processing using randomization as follows. (1) Content encoding. We propose to use hardware-based thread-private random numbers to encode the contents of the branch predictor tables. It achieves a similar effect of logical isolation but adds little in terms of space or time overheads. (2) Index encoding. We propose a randomized index mechanism of the branch predictor. This disrupts the correspondence between the branch instruction address and the branch predictor entry, thus increases the noise for malicious perception attacks. Our analyses using an FPGA-based RISC-V processor prototype and additional auxiliary simulations suggest that the proposed mechanisms incur a very small performance cost while providing strong protection.'
publication: '*DAC 2021*'
url_pdf: https://ieeexplore.ieee.org/abstract/document/9586178
doi: 10.1109/DAC18074.2021.9586178
---

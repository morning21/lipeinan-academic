---
# Documentation: https://wowchemy.com/docs/managing-content/

title: A Lightweight Isolation Mechanism for Secure Branch Predictors
subtitle: ''
summary: ''
authors:
- Lutan Zhao
- Peinan Li
- "[Rui Hou](http://hourui-arch.net/)"
- Michael C. Huang
- Jiazhen Li
- Lixin Zhang
- Xuehai Qian
- Dan Meng
tags: []
categories: []
date: '2020-01-01'
lastmod: 2020-11-30T23:51:00+08:00
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
publishDate: '2020-11-30T15:51:00.254843Z'
publication_types:
- '2'
abstract: 'Recently exposed vulnerabilities reveal the necessity to improve the security of branch predictors. Branch predictors record history about the execution of different programs, and such information from different processes are stored in the same structure and thus accessible to each other. This leaves the attackers with the opportunities for malicious training and malicious perception. Instead of flush-based or physical isolation of hardware resources, we want to achieve isolation of the content in these hardware tables with some lightweight processing using randomization as follows. (1) Content encoding. We propose to use hardware-based thread-private random numbers to encode the contents of the branch predictor tables (both direction and destination histories) which we call XOR-BP. Specifically, the data is encoded by XOR operation with the key before written in the table and decoded after read from the table. Such a mechanism obfuscates the information adding difficulties to cross-process or cross-privilege level analysis and perception. It achieves a similar effect of logical isolation but adds little in terms of space or time overheads. (2) Index encoding. We propose a randomized index mechanism of the branch predictor (Noisy-XOR-BP). Similar to the XOR-BP, another thread-private random number is used together with the branch instruction address as the input to compute the index of the branch predictor. This randomized indexing mechanism disrupts the correspondence between the branch instruction address and the branch predictor entry, thus increases the noise for malicious perception attacks. Our analyses using an FPGA-based RISC-V processor prototype and additional auxiliary simulations suggest that the proposed mechanisms incur a very small performance cost while providing strong protection.'
publication: '*CoRR*'
url_pdf: https://arxiv.org/abs/2005.08183
---

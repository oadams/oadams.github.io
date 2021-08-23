---
layout: post
title:  "Statistical Rethinking Solutions in Python/pymc3"
date:   2021-08-24 00:00:00 +1000
categories: statistics python
---

I recently found the need to apply a hierarchical Bayesian model in a project. That experience has motivated me to refine my Bayesian statistics skills. Years ago I used Gibbs sampling and a Dirichlet Process to sample distributions over phoneme/word alignments in finite state transducers [to improve speech recognition using written translations in another language](https://aclanthology.org/D16-1263.pdf). I learnt a lot doing this, however I mostly learnt all the relevant concepts on a need-to-know basis. This time I want to learn a more general understanding and set of skills from the ground up. It's very interesting, and having practical abilities with statistics is a timeless skill set.

I've been reading Richard McElreath's [Statistical Rethinking (2nd edition)](https://xcelab.net/rm/statistical-rethinking/) and have now started to work through the practice problems found at the end of each chapter. I'm using Python and pymc3 because life is short and want to leverage my existing Python skills and also practice the statistical skills using the language and libraries I would be using in real world projects. I thought it might be useful to publish my answers online, and so here they are. Note that I'm only including my answers, not the questions that were in the book itself. This will make these answers difficult to interpret without the book.

In my solutions I build upon the very [Python/pymc3 ports](https://github.com/pymc-devs/resources/tree/master/Rethinking_2) of the code examples in the book. Since the problems are designed to practice concepts learnt in their respective chapters, I have ended up making heavy use of the code from that repository, since their code frequently forms the scaffold to solutions to the problems.

I will update this post as I produce more solutions.

[Chapter 2 solutions](/statistical_rethinking_solutions/ch2.html)

[Chapter 3 solutions](/statistical_rethinking_solutions/ch3.html)

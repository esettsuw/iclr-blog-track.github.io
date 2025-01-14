---
layout: post
title: BackPACK (Packing more into Backprop)
tags: [Optimization]
authors: Dangel, Felix, University of Tuebingen; Kunstner, Frederik, University of Tuebingen; Hennig, Philipp, University of Tuebingen
---

# Abstract

Automatic differentiation frameworks are optimized for exactly one thing: computing the average mini-batch gradient. Yet, other quantities such as the variance
of the mini-batch gradients or many approximations to the Hessian can, in theory,
be computed efficiently, and at the same time as the gradient. While these quantities
are of great interest to researchers and practitioners, current deep-learning
software does not support their automatic calculation. Manually implementing
them is burdensome, inefficient if done na¨ıvely, and the resulting code is rarely
shared. This hampers progress in deep learning, and unnecessarily narrows research
to focus on gradient descent and its variants; it also complicates replication
studies and comparisons between newly developed methods that require
those quantities, to the point of impossibility. To address this problem, we introduce
BACKPACK1, an efficient framework built on top of PYTORCH, that extends
the backpropagation algorithm to extract additional information from first- and
second-order derivatives. Its capabilities are illustrated by benchmark reports for
computing additional quantities on deep neural networks, and an example application
by testing several recent curvature approximations for optimization.

# Introduction

BACKPACK is an efficient framework ...

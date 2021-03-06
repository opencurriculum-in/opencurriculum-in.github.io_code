---
title: "Singular Value Decomposition"
linkTitle: "Singular Value Decomposition"
weight: 3
---

Spectral Decomposition as we described it, only applies for symmetric square matrices. Singular value decomposition can be thought of as a generalization to non symmetric and non square matrices.

Given a matrix $M \in \mathbb R^{m\times n}$ which corresponds to a linear transformation $L:\mathbb R^n \rightarrow \mathbb R^m$. We can define two square matrices $MM^t \in \mathbb R^{m \times m}, M^tM \in \mathbb R^{n \times n}$ corresponding to it. 

{{< qapane >}}
{{< que >}}
Show that $MM^t \in \mathbb R^{m \times m}, M^tM \in \mathbb R^{n \times n}$ are symmetric.
{{< /que >}}
{{< ans >}}
Take transpose and verify.
{{< /ans >}}

{{< /qapane >}}

By Spectral Theorem there is an orthonormal eigenvector basis.
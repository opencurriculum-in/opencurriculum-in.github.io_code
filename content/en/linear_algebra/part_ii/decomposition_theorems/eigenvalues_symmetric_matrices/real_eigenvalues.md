---
title: "Eigenvalues of Symmetric Matrices are Real"
linkTitle: "Real Eigenvalues"
weight: 1
---
First lets try to prove this result for real symmetric matrices and then we will generalize the result to complex matrices.

## Real Symmetric Matrices

{{< definition title="Symmetric Matrix" >}}
$M \in \mathbb R^{n\times n}$ is _symmetric_ iff $M^t = M$.
{{< /definition >}}

{{< definition title="Orthonormal Matrix" >}}
$M \in \mathbb R^{n\times n}$ is _orthonormal_ if columns of $M$ are orthonormal.
{{< /definition >}}



{{< theorem num="1">}}
If $M$ is orthonormal then $M^{-1} = M^t$.
{{< /theorem >}}

{{< theorem num="2">}}
If $M$ is symmetric and $\lambda, v$ is any eigenvalue, eigenvector pair of $M$ as a matrix over the $\mathbb R$ then $v^t$ is a left eigenvector of $M$ with eigenvalue $\lambda$.
{{< /theorem >}}

_Proof:_ 

{{< qapane >}}
  {{< que >}}
What do we know?

What do we need to prove?
  {{< /que >}}

  {{< ans >}}
We are given that
$$ Mv = \lambda v \tag*{(1)}$$
and 
$$ M^t = M.$$
To prove that
$$ v^tM= \lambda v^t $$
  {{< /ans >}}

  {{< que>}}
What if we take the transpose of the equation $(1)$ on both sides.
$$ Mv = \lambda v \tag*{(1)}$$
  {{< /que >}}

  {{< ans >}}
$$
\begin{aligned}
\text{LHS} &= (Mv)^t = v^tM^t = v^tM\qquad (\text{Since } M = M^t)\cr
\text{RHS} &= \lambda v^t
\end{aligned}
$$
Hence $v^tM = \lambda v^t$.
  {{< /ans >}}
{{< /qapane >}}



{{< theorem num="3">}}
If $M$ is symmetric and $\lambda$ is any eigenvalue of $M$ as a matrix over the $\mathbb C$ field then $\lambda \in \mathbb R$.
{{< /theorem >}}

_Proof:_ 

{{< qapane >}}

{{< que >}}

Let $v$ be the eigenvector corresponding to $\lambda$. From the previous theorem, we know that $v^t$ is a left eigenvector for the same eigenvalue. Consider the expression
$$ \overline{v}^tMv.$$
We can expand it in two ways.

$$ = (\overline{v}^tM)v = \overline{v}^tMv = v^t(Mv) $$

{{< /que >}}
{{< ans >}}
{{< /ans >}}
{{< /qapane >}}


## Generalization to Complex Matrices

{{< definition title="Hermitian Matrix" >}}
$M \in \mathbb C^{n\times n}$ is called _Hermitian_ if $\overline{M}^t = M$.
{{< /definition >}}


{{< definition title="Unitary Matrix" >}}
$M \in \mathbb C^{n\times n}$ is _unitary_ if columns of $M$ are orthonormal under the complex dot product $\langle v, w \rangle = \overline{v}^t w$.
{{< /definition >}}



{{< theorem >}}
If $M$ is unitary then $M^{-1} = \overline{M}^t$.
{{< /theorem >}}

{{< theorem >}}
If $M$ is hermitian and $\lambda$ is any eigenvalue of $M$ then $\lambda \in \mathbb R$.
{{< /theorem >}}
_Proof:_

$$
\begin{align} 
\overline{v}^tMv &= \overline{v}^t(Mv) &= \lambda \overline{v}^tv \cr
& = (\overline{v}^tM)v = (\overline{v}^t\overline{M}^t)v =(\overline{Mv})^tv &=  \overline{\lambda}\overline{v}^tv 
 \end{align}
$$
From equations $(1), (2)$, $\lambda = \overline \lambda \Rightarrow \lambda \in \mathbb R$.
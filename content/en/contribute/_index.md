---
title: "Contribute"
linkTitle: "Contribute"
weight: 20
menu:
  main:
    weight: 25
---

<br/>
<br/>
<br/>
<br/>

Any of the course pages is editable on the web via links on the right sidebar.

# Format
The format is mostly markdown. Some additional syntax is provided for theorems, definitions and QA panels.

#### Definition
Following code
{{< highlight md >}}
{{</* definition title="Symmetric Matrix" */>}}
$M \in \mathbb R^{n\times n}$ is _symmetric_ iff $M^t = M$.
{{</* /definition */>}}
{{< / highlight >}}
is presented as:  

{{< definition title="Symmetric Matrix" >}}
$M \in \mathbb R^{n\times n}$ is _symmetric_ iff $M^t = M$.
{{< /definition >}}



#### Theorem
Following code
{{< highlight md >}}
{{</* theorem title="Spectral Theorem" num="1"*/>}}
Suppose $M \in \mathbb R^{n \times n}$.
$$M \text{ is symmetric } \iff M \text{ has an orthonormal eigen basis.}$$
{{</* /theorem */>}}
{{< / highlight >}}
is presented as:  
  
{{< theorem title="Spectral Theorem" num="1">}}
Suppose $M \in \mathbb R^{n \times n}$.
$$M \text{ is symmetric } \iff M \text{ has an orthonormal eigen basis.}$$
{{< /theorem >}}


#### QA Panel
Following code 
{{< highlight md >}}
{{</* qapane */>}}
  {{</* que */>}}
    What do we know?
    What do we need to prove?
  {{</* /que */>}}
  {{</* ans */>}}
    We are given that
    $$ Mv = \lambda v \tag*{(1)}$$
    and 
    $$ M^t = M.$$
    To prove that
    $$ v^tM= \lambda v^t $$
  {{</* /ans */>}}

  {{</* que */>}}
    What if we take the transpose of the equation $(1)$ on both sides.
    $$ Mv = \lambda v \tag*{(1)}$$
  {{</* /que */>}}
  {{</* ans */>}}
    $$
    \begin{aligned}
    \text{LHS} &= (Mv)^t = v^tM^t = v^tM\qquad (\text{Since } M = M^t)\cr
    \text{RHS} &= \lambda v^t
    \end{aligned}
    $$
    Hence $v^tM = \lambda v^t$.
  {{</* /ans */>}}
{{</* /qapane */>}}
{{< /highlight >}}
is presented as :  

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


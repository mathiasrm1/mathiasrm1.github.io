---
title: Measure Theory 3 Measurable Spaces and Functions
date: 2023-12-21 12:00:00 -500
categories: [measure theory]
tags: [measure theory, measurable functions, measurable spaces, borel sets, sigma algebras] #tags always lowercase
math: true
---

In the previous post we saw that the outer measure cannot satisfy lala, and we must restrict ourselves to certain sets.


>**Definition: $\sigma$-algebra**
> Suppose $X$ is a set and $\mathcal{S}$ is a collection of subsets of $X$, Then $\mathcal{S}$ is a $\sigma$-algebra if
>* $\varnothing  \in \mathcal{S}$
>* $E \in \mathcal{S} \text{ then } X \backslash E \in   \mathcal{S}$
>* $E_1, E_2...\in \mathcal{S}\text{ then } \bigcup_{i=1}^{\infty}E_i  $   

---
We can immediatly deduce another three desirable properties of $\sigma$-algebras:

#### Lemma: $\sigma$-algebra additional properties.
Suppose $\mathcal{S}$ is a $\sigma$-algebra on $X$. Then the following holds:
1. $X \in \mathcal{S}$. 
2. $D,E \in \mathcal{S}$ then $D\cup E \in \mathcal{S}$ and $D\cap E\in \mathcal{S}$ and $D\backslash E \in \mathcal{S}$
3. $E_1,E_2,... \in \mathcal{S}$ then $\bigcap_{i=1}^{\infty}  E_i \in \mathcal{S}$

#### Proof: 
Point 1. follows immediatly from the fact that $\varnothing \in \mathcal{S}$ and that $\sigma$-algebras are closed under complementation, so $X \backslash \varnothing = X \in \mathcal{S}$.

In point 2., proving $D\cup E \in \mathcal{S}$ follows from $\sigma$-algebras being closed under unions, setting $E_1=D$ and $E_2=E$, and $E_i=\varnothing$ for $i \geq 3$.

Showing $D\cap E \in \mathcal{S}$ is proven by considering De Morgan

$$ X\backslash (D\cap E) = (X\backslash D) \cup (X \backslash E),$$

and as both $X \backslash D, X\backslash E \in \mathcal{S}$ then $X\backslash (D\cap E)$. By the closed under complementation property we also have $D \cap E \in \mathcal{S}$. To prove $D \backslash E \in \mathcal{S}$, consider

$$D \backslash E = D \cap (X \backslash E). $$

Since we have shown $\sigma$-algebras are closed under finite intersections and both $D,(X \backslash E) \in \mathcal{S}$ then $D \backslash E \in \mathcal{S}$. 

To prove point 3. consider sequence $E_1, E_2,... \in \mathcal{S}$ and De Morgan

$$ X\backslash \bigcap_{i=1}^{\infty} E_i = \bigcup_{i=1}^{\infty}(X\backslash E_i). $$

As the right hand side is an element of $\mathcal{S}$ (by closed under complementation and closed under coutable unions)  we have 

$$ X\backslash (X\backslash \bigcap_{i=1}^{\infty} E_i) = \bigcap_{i=1}^{\infty} E_i  $$

and thus $\bigcap_{i=1}^{\infty} E_i \in \mathcal{S}$.

$$\tag*{$\blacksquare$}$$





> #### Definition: Measureable space and Measurable sets
> * A measurable space is an ordered pair $(X,\mathcal{S})$, where $X$ is a set and $\mathcal{S}$ a $\sigma$-algebra on $X$.
>* An element of $\mathcal{S}$ is called a $\mathcal{S}$-measurable set or simply a measurable set whenever the $\sigma$-algebra is clear from context.

Note: The notation of a measurable space and measure space are different. A measure space is a triple, also inculding a measure, which is the subject of the next chapter.



### Borel Subsets of $\mathbb{R}$

The next result guarantees the existence of a smallest $\sigma$-algebra on a set $X$ containing a given set $\mathcal{A}$ of subsets of $X$. This result is quite analoguous to what we are familiar with from topology. In topology, we recall that given a set of subsets $\mathcal{S}$ of $X$ then there exists a unique topology denoted $\langle\mathcal{S}\rangle$, which is the coarsest (the smallest topology. i.e. containing the fewest open sets) topology containing $\mathcal{S}$. 


#### Lemma: Smallest $\sigma$-algebra containing a collection of subsets
Suppose $X$ is a set and $\mathcal{A}$ is a set of subsets of $X$. Then the intersection of all $\sigma$-algebras on $X$ that contain $\mathcal{A}$ is a $\sigma$-algebra on $X$.

#### Proof: 

* TO
* BE
* WRITTEN

$$\tag*{$\blacksquare$}$$

Now a crucial definition

>#### Definition: Borel $\sigma$-algebra and Borel sets
>The smallest $\sigma$-algebra containing all open subsets of $\mathbb{R}$ is called the Borel $\sigma$-algebra, an element of this $\sigma$-algebra is called a Borel set.

#### Example: Borel sets


Link to inverse images post




### Measurable Functions


> ### Definition: Measurable Functions
> Suppose $(X,\mathcal{S})$ is a measurable space. A function $f\colon X \to \mathbb{R}$ is called $\mathcal{S}$-measurable(or measurable) if 
>$$ f^{-1}(B) \in \mathcal{S}$$
> for any Borel set $B \subset \mathbb{R}$


### Example: Measurable functions













Exercise: lalal

<details>
  <summary>Solution</summary>
  2+2=4

</details>


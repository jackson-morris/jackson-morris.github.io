---
layout: archive
title: "A user's guide: Rings of cooperations for Hermitian K-theory over finite fields"
permalink: /guides/finitekqcooperations
author_profile: true
---

**Source paper:** [Rings of cooperations for Hermitian K-theory over finite fields](https://arxiv.org/abs/2509.02786)

**Source abstract:** We compute the ring of cooperations $\pi_{**}^{\mathbb{F}_q}(\text{kq} \otimes \text{kq})$ for the very effective Hermitian K-theory over all finite fields $\mathbb{F}_q$ where $\text{char}(\mathbb{F}_q) \neq 2$. To do this, we use the motivic Adams spectral
sequence and show that all differentials are determined by the integral motivic cohomology of $\mathbb{F}_q$.
As an application, we compute the $\text{E}_1$-page of the $\text{kq}$-resolution.

Background on the problem
===
The background on this problem is the same as the background for the case of $F=\mathbb{R}$, which I wrote about [here](guide_real_kq_coop.md). The only difference is that, instead of computing over $\mathbb{C}$ or $\mathbb{R}$, I just chose to compute in $\text{SH}(\mathbb{F}_q)$. The motivation for working over finite fields is two-fold:

* The program to compute the cooperations $\pi_{**}^{F}(\text{kq} \otimes \text{kq})$ is essentially algorithmic; see 
[this document](/files/Splittings_and_the_algebraic_Atiyah_Hirzebruch_spectral_sequence%20(2).pdf) to see what I mean in the classical case. The only hard input one needs to run this algorithm is a computation of the motivic cohomology of the subalgebra $A(1)$ of the motivic Steenrod algebra and/or (often coinciding with but not always) the homotopy groups of the very effective Hermitian K-theory spectrum $\text{kq}$. This has been computed over all finite fields of characteristic different from 2 by Kylling and Wilson, and so serves as some necessary input. I don't think there are any other computations of this input over other base fields (yet), but I think computing over $\mathbb{Q}$ or some $p$-adic field is certainly doable.

* [Work of Bachmann-Østvær](https://arxiv.org/abs/2102.01618) determines that, after 2-completion, if $X$ is some cellular motivic spectrum over $\mathbb{Z}[1/2]$, then there is an equivalence between the mapping spectrum $X(\mathbb{Z}[1/2])$ and the pullback along the base-change maps $X(\mathbb{F}_3) \times_{X(\mathbb{C})}X(\mathbb{R})$. In particular, this situates cellular computations over $\mathbb{Z}[1/2]$ in a Mayer-Vietoris style long exact sequence with analogous computations over $\mathbb{R}, \mathbb{C}$, and $\mathbb{F}_3$. This is pretty wacky, and I have loads more to say about this (is this an equivalence of categories??), but the real influence this had on the paper at hand was that if I can compute the ring of cooperations over $\mathbb{F}_3$, then using my previous computation over $\mathbb{R}$ and Culver-Quigley's computation over $\mathbb{C}$, I can try to long exact sequence my way to an integral computation.

What this paper does
===
**The short of it**

I computed the $\text{E}_1$-page of the $\text{kq}$-resolution over finite fields of characteristic different from 2. So, this involves a computation (modulo some irrelavent $v_1$-torsion) of
$$\pi_{**}^{\mathbb{F}_q}(\text{kq} \otimes \text{kq}^{\otimes *}).$$
Unlike in previous cases, there are some interesting differentials.

**The long of it**

This is really similar in spirit to my previous paper. It formally follows the same algorithm, but there are some slight differences that appear on a case by case basis. For one, there are two cases to consider at hand: when $q \equiv 1 \, (4)$ or when $q \equiv 3 \, (4)$. The input to this computation involves Ext over the Steenrod algebra, and the Steenrod algebra acts differently in both cases.

The most interesting difference or new occurence here, previously unseen in the $\text{kq}$-cooperations world, is some differentials in the Adams spectral sequence! The point is that you can kinda build everything in sight out of cofiber sequences. We have

$$\text{H}\mathbb{Z} \to \text{H}\mathbb{Z} \to \text{H}\mathbb{F}_2$$

$$\Sigma^{2,1}\text{kgl} \to \text{kgl} \to \text{H}\mathbb{Z}$$

$$\Sigma^{1,1}\text{kq} \to \text{kq} \to \text{kgl}.$$

And indeed, one way to interpret some of these computations is by starting at the $\text{H}\mathbb{Z}$-cooperations case, $v_1$-Bockstein-ing to the $\text{kgl}$ case, and then $\eta$-Bockstein-ing to the $\text{kq}$ case. This perspective illuminates where the differentials are coming from. The homotopy of $\text{H}\mathbb{Z}$ is determined by the integral motivic homology of the base field, which was determined by Suslin back in the 80s. One can calculate the $\text{E}_2$-page of the Adams spectral sequence computing the homotopy of $\text{H}\mathbb{Z}$, and knowing what we are converging to forces the differential pattern.

It turns out that these differentials are the only differentials that lift to the Adams spectral sequence computing either the homotopy of $\text{kq}$ or the homotopy of the cooperations! Another fun consequence is that I was able recompute Friedlander's computation of the symplectic K-theory of finite fields using the Adams spectral sequence.


How did this all come together?
===
After I computed the $\mathbb{R}$-motivic ring of cooperations, I wasn't sure what to do next. Should I go ahead and try to compute the $\text{kq}$-resoultion and say something about motivic $v_1$-periodicity? Should I move on to an entirely new project? I settled on a third point: expand the class of base schemes on which we have a comptuation of the ring of cooperations, or really the whole $\text{E}_1$-page of the $\text{kq}$-resolution. This was the next natural step. It honestly came together very quickly and was much more fun than the $\mathbb{R}$-motivic analogue. The arithmetic coming out was very interesting.


What's next?
===
No idea. Lots of directions, lots of decisions.
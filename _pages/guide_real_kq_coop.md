---
layout: archive
title: "A user's guide: On the ring of cooperations for real Hermitian K-theory"
permalink: /guides/realkqcooperations
author_profile: true
---

**Source paper:** [On the ring of cooperations for real Hermitian K-theory](https://arxiv.org/abs/2506.16672)

**Source abstract:** Let $\text{kq}$ denote the very effective cover of the motivic Hermitian K-theory spectrum. We analyze the ring of cooperations $\pi_{**}^\mathbb{R}(\text{kq} \otimes \text{kq})$ in the stable motivic homotopy category $\text{SH}(\mathbb{R})$, giving a full description in terms of Brown--Gitler comodules. To do this, we decompose the $\text{E}_2$-page of the motivic Adams spectral sequence and show that it must collapse. The description of the $\text{E}_2$-page is accomplished by a series of algebraic Atiyah--Hirzebruch spectral sequences which converge to the summands of the $\text{E}_2$-page. Along the way, we prove a splitting result for the very effective symplectic K-theory $\text{ksp}$ over any base field of characteristic not two.

Background on the problem
===
*Classical motivation: Mahowald knew everything*

A central question in homotopy theory is to understand the stable homotopy groups of spheres $\pi_*\mathbb{S}$. By understand, I mean to compute the groups $\pi_k\mathbb{S}$ for all $k \geq 0$ and to study the relationship that the elements of this group have with each other. Starting with the first point, work of Serre tells us that $\pi_k\mathbb{S}$ is a finite abelian group for all $k>0$. This allows us to work one prime at a time, computing only the $p$-typical component of each stable stem. The sphere spectrum is the monoidal unit for the smash product on spectra, which gives $\pi_*\mathbb{S}$ the structure of a graded ring. However, Nishida's theorem tells us that if $x \in \pi_k\mathbb{S}$ for any $k>0$, then $x$ is nilpotent. In other words, the ring structure on $\pi_*\mathbb{S}$ is garbage.

In the 60s, Adams constructed infinite families of elements in $\pi_*\mathbb{S}$. These families do not live in one particular degree, so they do not break Serre's finiteness result, nor are they direct multiples of each other, so they do not break Nishida's nilpotence theorem. This was the birth of chromatic homotopy theory, which extends Adams ideas and organizes the elements of $\pi_*\mathbb{S}$ into $v_n$-periodic families for $n \geq 0$. One should think of these $v_n$'s as "higher primes" which only become visible after killing the previous one. By pioneering work of Morava, Quillen, and many others, it was discovered that the periodic behavior of the stable stems are controlled by the moduli stack of formal groups, which allows one to study homotopy theory using tools from arithmetic geometry. It's really incredible, although I won't talk about this connection very much.

The $v_0$-periodic layer of $\pi_*\mathbb{S}$ is just the rationalization. By Serre's finiteness, the only $v_0$-periodic elements in $\pi_*\mathbb{S}$ are those in $\pi_0\mathbb{S} \cong \mathbb{Z}$. The elements constructed by Adams are a part of the $v_1$-periodic layer. Note that, implicitely, we are working one prime at a time now, and for the rest of this guide we will be working at the prime 2. These elements are deeply related to topological K-theory and are more mysterious than the $v_0$-periodic ones. This gives us a question:

**What are the $v_1$-periodic elements of $\pi_*\mathbb{S}$?**

The whole point to this introduction is that we actually know the answer to the above question, and it was all due to bunch of different ideas floating around with Mahowald. I'll streamline what he did in "bo-resolutions" - sorry if you wanted hear anything about the J-homomorphism!

The best tool we have to compute homotopy groups is the Adams spectral sequence. For a spectrum $\text{E}$, this takes the form
$$\text{E}_1^{s,f} = \pi_{s+f}(\text{E} \otimes \overline{\text{E}}^{\otimes f}) \implies \pi_s\mathbb{S}.$$
The classical Adams spectral sequence, taking $\text{E}=\text{H}\mathbb{F}_2$ the Eilenberg-MacLane spectrum for $\mathbb{F}_2$-cohomology, actually starts at the $\text{E}_2$-page:
$$\text{E}_2^{s,f} = \text{Ext}_{\mathcal{A}^\vee}^{s,f}(\mathbb{F}_2, \mathbb{F}_2) \implies \pi_s\mathbb{S}.$$
In general, however, one actually needs to start with the $\text{E}_1$-page.

Different choices of $\text{E}$ have Adams spectral sequences which are good for different purposes. The $\text{H}\mathbb{F}_2$-based Adams spectral sequence is great for computing $\pi_*\mathbb{S}$ stem-by-stem, but not so good at quickly identifying periodic elements. Mahowald's realization was the following: the connective topological K-theory spectrum $\text{bo}$ has an element $v_1^4 \in \pi_8\text{bo}$ in its homotopy, which is useful in showing that Adams families of elements are nonzero. It ought to be the case that the $\text{bo}$-based Adams spectral sequence is good at isolating the $v_1$-periodic part of $\pi_*\mathbb{S}$!

This is true. This is the whole point: Mahowald's analysis of the $\text{bo}$-resolution allows one to completely identify the $v_1$-periodic part of the stable stems. His results were then shown to imply the height 1 telescope conjecture, which equates two rivaling methods to access $v_1$-periodic homotopy. I should remark that it is partially on the basis of this computation, as well as Haynes Miller's in the odd primary case, that lead to Ravenel even forming the telescope conjecture in the first place. Additionally, we now know that this is the only positive height at which the telescope conjecture is even true!

*Motivic homotopy theory from the perspective of homotopy theory*

What this paper does
===

How did this all come together?
===

What's next?
===
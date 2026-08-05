---
layout: archive
title: "A user's guide: Splittings of truncated motivic Brown-Peterson cooperation algebras"
permalink: /guides/bpgl1cooperations
author_profile: true
---

**Source paper:** [Splittings of truncated motivic Brown-Peterson cooperations algebras](https://arxiv.org/abs/2509.19542)

**Source abstract:** We construct spectrum-level splittings of BPGL⟨1⟩∧BPGL⟨1⟩ at all primes p, where BPGL⟨1⟩ is the first truncated motivic Brown--Peterson spectrum. Classically, BP⟨1⟩∧BP⟨1⟩ was first described by Kane and Mahowald in terms of Brown-Gitler spectra. This splitting was subsequently reinterpreted by Lellman and Davis-Gitler-Mahowald in terms of Adams covers. In this paper, we give motivic lifts of these splittings in terms of Adams covers, over the base fields ℂ,ℝ, and 𝔽q, where 𝔽q≠p. As an application, we compute the E1-page of the BPGL⟨1⟩-based Adams spectral sequence as a module over BPGL⟨1⟩, both in homotopy and in terms of motivic spectra. We also record analogous splittings for BPGL⟨0⟩∧BPGL⟨0⟩

Background on the problem
===
Inspiration for these splitting-style results comes from a few places, but my primary motivation is that one would like to understand the $E$-based motivic Adams spectral sequence, which has signature

$$
    E_1 = \pi_{s+f,w}(E\otimes\overline{E}^{\otimes f}) \implies \pi_{s,w}^F(\mathbb{S}).
$$

A splitting of $E\otimes E$ gives a much better understanding of this $E_1$-page. The particular choice of motivic spectrum $E$ may be better equipped at seeing different parts of the homotopy of the sphere spectrum.

For instance, at the prime 2, the motivic Adams spectral sequence based on the very effective hermitian K-theory spectrum $kq$, called the $kq$-resolution, is pretty good at distinguishing the $v_1$-periodic component (this is certainly true over $\mathbb{C}$, and is conjecturally true over other fields). My previous two papers had investigated this spectral sequence over the real numbers and finite fields. 

Contrary to common belief, there are in fact other primes than just 2! The purpose of this paper is to analyze the motivic Adams spectral sequence based on a spectrum $E$ which is good at seeing $v_1$-periodicity at odd primes. As some motivation, a specturm which holds a lot of the secrets of $v_1$-periodicity is the motivic Lubin Tate spectrum $E_1^{mot}$, which is modeled by the $p$-complete algebraic K-theory spectrum $KGL$. This spectrum admits an action by $\mathbb{Z}^{\times}\_{p}$, the Adams operations. Taking fixed points for this action brings one closer to the sphere, in that the unit map $\mathbb{S} \to E_1^{mot}$ factors through the fixed points. For $p=2$, a maximal finite subgroup of $\mathbb{Z}^{\times}\_2$ is $C_2$, and the homotopy fixed points are $KGL^{hC_2}\simeq KQ$, whose appropriate cover in motivic homotopy theory is the very effective hermitian K-theory $kq$. For $p$ odd, a maximal finite subgroup of $\mathbb{Z}^{\times}\_p$ is $C_{p-1}$, and the homotopy fixed points are $KGL^{hC_{p-1}}\simeq E(1)$, whose appropriate cover in motivic homotopy theory is the truncated Brown--Peterson spectrum $BPGL\langle 1\rangle$. This spectrum is often called the motivic Adams summand $m\ell$. At the prime 2, $BPGL\langle 1 \rangle \simeq kgl$, the effective algebraic K-theory spectrum.

What this paper does
===
Sarah, Liz and I do a lot of things in this paper! We first compute the homotopy cooperations $\pi_{**}BPGL\langle 1 \rangle\otimes BPGL\langle 1 \rangle$, then extend our techniques to describe the $E_1$-page of the $BPGL\langle 1 \rangle$-based motivic Adams spectral sequence. We make these computations at all primes, and over the complex bumbers, real numbers, and finite fields. Inspired by work of Gonzales, this should see a lot of $v_1$-periodicity in the sphere!

Here's what's really surprising and cool. There are no topological splittings of $kq\otimes kq$, which kinda sucks. These splittings would be made in terms of Brown-Gitler spectra, and there are curretnyly no construction of motivic Brown-Gitler spectra. For the case of $BPGL\langle 1 \rangle \otimes BPGL \langle 1 \rangle$, we kinda just bypass this problem! We are able to make a splitting in terms of Adams covers. This type of splitting is also not available for $kq \otimes kq$, and highlights that $v_1$-periodicity in motivic homotopy theory is simpler to understand at odd primes. There are a bunch of charts that I kinda went hogwild making for this paper. I am really proud of them, for whatever reason.

We also make analogous computations in the case of $BPGL\langle 0 \rangle \simeq H\mathbb{Z}_{p}$.


What's next?
===
I have spent a bunch of time computing the $E_1$-page of various motivic Adams spectral sequences. I would really like to compute these Adams spectral sequences!!

Unfortunately, I am a bit of a completionist. Sarah, Liz and I are running through the $kgl$ and $kq$ cooperations gauntlet over $\mathbb{Q}_p$ and $\mathbb{Q}$ first. These computations are similar in spirit to what I have previously done, but involve some more technical arithmetic which is very annoying/interesting. 
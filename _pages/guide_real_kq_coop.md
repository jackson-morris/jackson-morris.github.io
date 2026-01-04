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

A central task in homotopy theory is to understand the stable homotopy groups of spheres $\pi_*\mathbb{S}$. By understand, I mean to compute the groups $\pi_k\mathbb{S}$ for all $k \geq 0$ and to study the relationship that the elements of this group have with each other. Starting with the first point, work of Serre tells us that $\pi_k\mathbb{S}$ is a finite abelian group for all $k>0$. This allows us to work one prime at a time, computing only the $p$-typical component of each stable stem. The sphere spectrum is the monoidal unit for the smash product on spectra, which gives $\pi_*\mathbb{S}$ the structure of a graded ring. However, Nishida's theorem tells us that if $x \in \pi_k\mathbb{S}$ for any $k>0$, then $x$ is nilpotent. In other words, the ring structure on $\pi_*\mathbb{S}$ is garbage.

In the 60s, Adams constructed infinite families of elements in $\pi_*\mathbb{S}$. These families do not live in one particular degree, so they do not break Serre's finiteness result, nor are they direct multiples of each other, so they do not break Nishida's nilpotence theorem. This was the birth of chromatic homotopy theory, which extends Adams ideas and organizes the elements of $\pi_*\mathbb{S}$ into $v_n$-periodic families for $n \geq 0$. One should think of these $v_n$'s as "higher primes" which only become visible after killing the previous one. By pioneering work of Morava, Quillen, and many others, it was discovered that the periodic behavior of the stable stems are controlled by the moduli stack of formal groups, which allows one to study homotopy theory using tools from arithmetic geometry. It's really incredible, although I won't talk about this connection very much.

The $v_0$-periodic layer of $\pi_*\mathbb{S}$ is just the rationalization. By Serre's finiteness, the only $v_0$-periodic elements in $\pi_*\mathbb{S}$ are those in $\pi_0\mathbb{S} \cong \mathbb{Z}$. The elements constructed by Adams are a part of the $v_1$-periodic layer. Note that, implicitely, we are working one prime at a time now, and for the rest of this guide we will be working at the prime 2. These elements are deeply related to topological K-theory and are more mysterious than the $v_0$-periodic ones. This gives us a question:

**What are the $v_1$-periodic elements of $\pi_*\mathbb{S}$?**

The whole point to this introduction is that we actually know the answer to the above question, and it was all due to bunch of different ideas floating around with Mahowald. I'll streamline what he did in "bo-resolutions" - sorry if you wanted hear anything about the J-homomorphism!

The best tool we have to compute homotopy groups is the Adams spectral sequence. For a spectrum $\text{E}$, this takes the form
$$\text{E}_1^{s,f} = \pi_{s+f}(\text{E} \otimes \overline{\text{E}}^{\otimes f}) \implies \pi_s\mathbb{S}.$$
The classical Adams spectral sequence, taking $\text{E}=\text{H}\mathbb{F}_2$ the Eilenberg-MacLane spectrum for $\mathbb{F}_2$-cohomology, actually starts at the $\text{E}_2$-page:
$$\text{E}_2^{s,f} = \text{Ext}_{\mathcal{A}^\vee}^{s,f}(\mathbb{F}_2, \mathbb{F}_2) \implies \pi_s\mathbb{S},$$
where $\mathcal{A}^\vee :=\pi_*(\text{H}\mathbb{F}_2 \otimes \text{H}\mathbb{F}_2)$ is the dual Steenrod algebra. In general, however, one actually needs to start with the $\text{E}_1$-page.

Different choices of $\text{E}$ have Adams spectral sequences which are good for different purposes. The $\text{H}\mathbb{F}_2$-based Adams spectral sequence is great for computing $\pi_*\mathbb{S}$ stem-by-stem, but not so good at quickly identifying periodic elements. Mahowald's realization was the following: the connective topological K-theory spectrum $\text{bo}$ has an element $v_1^4 \in \pi_8\text{bo}$ in its homotopy, which is useful in showing that Adams families of elements are nonzero. It ought to be the case that the $\text{bo}$-based Adams spectral sequence is good at isolating the $v_1$-periodic part of $\pi_*\mathbb{S}$!

This is true. This is the whole point: Mahowald's analysis of the $\text{bo}$-resolution allows one to completely identify the $v_1$-periodic part of the stable stems. His results were then shown to imply the height 1 telescope conjecture, which equates two rivaling methods to access $v_1$-periodic homotopy. I should remark that it is partially on the basis of this computation, as well as Haynes Miller's in the odd primary case, that lead to Ravenel even forming the telescope conjecture in the first place. Additionally, we now know that this is the only positive height at which the telescope conjecture is even true!

*Motivic homotopy theory: from the perspective of homotopy theory*

Motivic homotopy theory, as pioneered by Morel-Voevodsky, gives a way to study algebro geometric objects using tools from homotopy theory. The broad strokes are as follows. Take the category $\text{Sm}_F$ of smooth schemes over a field $F$. These are the "algebro-geometric objects we want to do homotopy theory with". The problem is that $\text{Sm}_F$ is not well behaved categorically, for instance not admitting all colimits, and a major innovation of motivic homotopy theory is the development of a good category of motivic spaces $\text{Spc}_F$. For technical reasons, this category has a bigraded family of spheres $S^{s,w}$. I like to think of the $s$ degree as the "stem" degree and the $w$ degree as the motivic weight.

From a nice category of motivic spaces, we may pass to the stable motivic homotopy category $\text{SH}(F)$, objects of which are called motivic spectra. The motivic sphere spectrum $\mathbb{S}$ is equivalent to $\Sigma_+^\infty\text{Spec}(F)$, and the stable motivic homotopy groups of spheres $\pi_{**}^F\mathbb{S}$ contain a mix of topological and arithmetic information about the base field $F$. 

The point here is not to reinent the wheel. Mahowald identifed a whole chunk of interesting of information in the topological stable stems using the $\text{bo}$-resolution. There is a motivic spectrum called the very effective Hermitian K-theory $\text{kq}$, which has connections to geometry that are not going to come up; all we need to know is that it contains an element $v_1^4 \in \pi_{8,4}^F\text{kq}$. The motivation for this paper is to determine the $v_1$-periodic part of $\pi_{**}^F\mathbb{S}$ by way of the $\text{kq}$-resolution.

Now comes a bit of choice: what field $F$ should one work over? From a computational perspective, working over $\mathbb{C}$ is the simplest. Culver-Quigley did this already, to great avail! They analogized the entirety of Mahowald's story, bypassing some hurdles that I will explain later, although there is a slight snag in the application to the telescope conjecture. So, what comes next? Well, in my case at least, it was $\mathbb{R}$. 

What this paper does
===
*The short of it*

This paper begins the study of the $\text{kq}$-resolution in $\mathbb{R}$-motivic homotopy theory. This spectral sequence takes the form
$$\text{E}_1^{s,f,w} = \pi_{s+f, w}^\mathbb{R}(\text{kq} \otimes \overline{\text{kq}}^{\otimes f}) \implies \pi_{s,w}^\mathbb{R}\mathbb{S}.$$
The first step to studying this resolution is just computing and understanding the $\text{E}_1$-page, which is significantly harder than either the classical or $\mathbb{C}$-motivic analogue. This is the main content of my paper: I computed the $\text{E}_1$-page of the $\text{kq}$-resolution, modulo some irrelevant $v_1$-torsion.

*The long of it*

One of the main tools that Mahowald uses in his classical arguments are Brown-Gitler spectra. These are finite spectra $\text{H}\mathbb{Z}_k$ for $k \geq 0$ which give rise to a splitting of the cooperations algebra:
$$\text{bo} \otimes \text{bo} \simeq \bigoplus_{k \geq 0}\Sigma^{4k}\text{bo} \otimes \text{H}\mathbb{Z}_k.$$
This topological splitting makes a lot of arguments run really smoothly.

There is currently no construction of motivic Brown-Gitler spectra. This is one of the biggest hurdles in this paper. To compute the homotopy ring of cooperations $\pi_{**}^\mathbb{R}(\text{kq} \otimes \text{kq})$, the bottom piece of the $\text{kq}$-resolution, we can use the mod-2 Adams spectral sequence:
$$\text{E}_2^{s,f,w} = \text{Ext}^{s,f,w}_{\mathcal{A}^\vee}(\mathbb{M}_2, \text{H}_{**}(\text{kq} \otimes \text{kq})) \implies \pi_{**}^\mathbb{R}(\text{kq} \otimes \text{kq})$$
where $\mathbb{M}_2 = \text{H}_{**}(\mathbb{S})$. One can show that there is a Kunneth isomorphism
$$\text{H}_{**}(\text{kq} \otimes \text{kq}) \cong \text{H}_{**}(\text{kq}) \otimes_{\mathbb{M}_2}\text{H}_{**}(\text{kq}).$$
Using the identification of $\mathcal{A}^\vee$-comodules $\text{H}_{**}(\text{kq}) \cong (\mathcal{A}//\mathcal{A}(1))^\vee$, we can use a change of rings isomorphism to rewrite the $\text{E}_2$-page of the above Adams spectral sequence as
$$\text{Ext}_{\mathcal{A}(1)^\vee}^{s,f,w}(\mathbb{M}_2, \text{H}_{**}(\text{kq})).$$
This is the point where having Brown-Gitler spectra would be useful. This would give us a way to rewrite this Ext group once again into smaller pieces that we can stitch together to give our final answer.

What I do is produce an algebraic splitting. There are comodules over the dual Steenrod algebra known as the Brown-Gitler comodules $B_0(k)$ which give rise to a splitting of $\mathcal{A}(1)^\vee$-comodules
$$\text{H}_{**}(\text{kq}) \cong \bigoplus \Sigma^{4k, 2k}B_0(k).$$
So, we can once again rewrite the Ext group using this algebraic splitting. Our question is reduced to computing the Ext groups
$$\text{Ext}_{\mathcal{A}(1)^\vee}^{s,f,w}(\mathbb{M}_2, B_0(k)).$$
This is really where most of the work in this paper is. We can filter these finite comodules by degree, giving rise to algebraic Atiyah-Hirzebruch spectral sequences whose differentials are determined by the $\mathcal{A}(1)^\vee$-comodule structure on $B_0(k)$. It takes a long time, there are a lot of charts, and it is kinda annoying.

The upshot is that once you have finally computed the $\text{E}_2$-page of the mod-2 Adams spectral sequence computing the cooperations, you've done so much work that you completely understand the $\text{E}_2$-page and can easily see that there is no room for differentials. What's nicer: this argument immediately extends to show that the mod-2 Adams spectral sequence
$$\text{E}_2^{s,f,w} = \text{Ext}_{\mathcal{A}^\vee}^{s,f,w}(\mathbb{M}_2, \text{H}_{**}(\text{kq} \otimes \overline{\text{kq}}^{\otimes f})) \implies \pi_{s, w}^\mathbb{R}(\text{kq} \otimes \overline{\text{kq}}^{\otimes f}),$$
which computes the $f$-line of the $\text{kq}$-resolution, is similarly decomposable and must also collapse at $\text{E}_2$. Thus, we have a full description of the $\text{E}_1$-page of the $\text{kq}$-resolution.

The downside, or why this problem was realyl so difficult, was that the Adams charts for this project are monstrously large. Even displaying the homotopy groups $\pi_{**}^\mathbb{R}\text{kq}$ in any reasonable way requires hree simultaneous charts. This means that, for example, keeping track of all of the data through one of the algebraic Atiyah-Hirzebruch spectral sequences required a total of 12 different charts, 3 for each page. It was and is a mess!

Something else I will add: there is a construction of the first motivic Brown-Gitler spectrum $\text{H}\mathbb{Z}_1$, and I also showed that there is an equivalence
$$\text{ksp} \simeq \text{kq} \otimes \text{H}\mathbb{Z}_1$$
where $\text{ksp}$ is the effective symplectic K-theory spectrum. This is a pretty neat argument involving the slice tower, and actually holds over any base scheme.

How did this all come together?
===
Sometime at the beginning of my third year of graduate school, my advisor, Kyle Ormsby, told me to think about $\text{kq} \otimes \text{kq}$. I didn't really know what he meant by this. Did he mean compute the homotopy groups of $\text{KQ} \otimes \text{KQ}$? Do something with slices? I had no real idea, and I didn't have any context for the question either. 

It took me about a year of messing around and going down a bunch of different rabbit holes to get to where I felt confident enough to start working on the project.
* I first tried to compute the homotopy groups of $\text{KQ} \otimes \text{KQ}$ using some type or arithmetic fracture square for the $C_2 \times C_2$-action on $\text{KGL} \otimes \text{KGL}$. I got nowhere. I then tried to imitate Adams-Harris-Switzer and how they computed the homotopy groups of $\text{KO} \otimes \text{KO}$. I got nowhere. I was really trying to use chromatic methods, as I was learning classical chromatic homotopy theory, and that machinery isn't really available or as straightforwards in the motivic case.
* I next tried to compute the slices of $\text{KQ} \otimes \text{KQ}$, mimicing the techniques of Pelaez-Weibel for computing the slices of $\text{KGL} \otimes \dots \otimes \text{KGL}$. Their techniques really leverage the fact that $\text{KGL}$ is an oriented motivic spectrum, though, and is not immediately ammenable to the $\text{KQ}$-case. So, in another way, I got nowhere.
* I then decided on computing $\pi_{**}(\text{kq}\otimes \text{kq})$. I didn't know much about this story. I looked at Behrens-Ormsby-Stapleton-Stojanoska's treatment of $\text{bo}_*\text{bo}$ for inspiration, and kinda got lost in the numerical polynomials nonsense, before deciding to push through with the Adams spectral sequence.

I then found Culver-Quigley's "kq-resolutions I", which computes the $\text{kq}$-resolution over $\mathbb{C}$. I didn't read the fine print at first, though, and thought that they had made their computation over any base scheme and that I had no problem! Luckily, I was wrong, and Kyle suggested I compute $\pi_{**}^\mathbb{R}(\text{kq} \otimes \text{kq})$ as a first step towards real $\text{kq}$-resolutions.

I began really thinking about this problem in my fourth year. Most of my third year was spent in this trial-and-error mode, which was actually a nice way to walk through the literature in homotopy theory. Once I started actually working on this problem, I was able to hone in on my literature searches. I read a ton of papers, a lot of them being from Mahowald or Behrens, and spent a lot of time confused. I had a lot of help from Kyle, John, and J.D., and from anyone in the UW mathematics department who would listen. I eventually got to a place where I needed to run some gnarly spectral sequences, and to have more space I bought a humongous book of graph paper. This big paper is the reason I finished this project!

There are a lot of charts in the paper, something like 30 in total. These are my favorite part of the project: learning how these charts worked helped me to understand the problem, communicate my answer, and shaped how I view homotopy theory as a whole. 

What's next?
===
There are a lot places I want to take this project! I'd love to actually compute the $\text{kq}$-resolution over the real numbers, and solve the $v_1$-periodic telescope conjecture. I've since tackled this problem over $\mathbb{F}_q$, and would be interested in working over other base schemes. It's just a fun computation and, at least to me, a beautiful story.
---
layout: archive
title: "Spectral sequences"
permalink: /sseq/
author_profile: true
---

On this page are open problems and resources for spectral sequences. The resources that I find most useful on this topic tend to be examples in papers and write ups from random graduate students.

Open Problems
=====
In progress

Personal Favorites
=====
In Progress


Topics
=====
* **Adams Spectral Sequence**
    <details>
    <summary>See more</summary>
    The (mod-p) Adams spectral sequence is the grandaddy of them all.
    <ul>
    <li><a href ="https://www.ms.uky.edu/~guillou/S24/751Notes.pdf">Chromatic homotopy theory</a>, Bert Guillou. Chapters 6 and 7 of these lecture notes have some great charts and background, and at odd primes.
    </li>
    <li><a href ="https://www.mn.uio.no/math/personer/vit/rognes/kurs/mat9580v12/notes.050612.pdf">The Adams Spectral Sequence</a>, John Rognes. Almost overwhelming in how much is covered in these notes.
    </li>
    <li><a href ="https://www.mn.uio.no/math/personer/vit/rognes/kurs/mat9580v15/adams-sp-seq.010615.pdf">Introduction to the Adams Spectral Sequence</a>, John Rognes. Different from the above Rognes entry but also incredible.
    </li>
    <li><a href ="https://amathew.wordpress.com/tag/adams-spectral-sequence/">Climbing Mount Bourbaki</a>, Akhil Mathew. This feels like reading someone's personal notebook, and I found it very useful to get my hands dirty for the first time.
    </li>
    <li><a href ="https://www.sas.rochester.edu/mth/sites/doug-ravenel/otherpapers/Beaudry-Campbell.pdf">A guide for computing stable homotopy groups</a>, gnes Beaudry and Jonathan Campbell. Nice introduction, cool cell diagrams.
    </li>
    <li><a href="https://www.sas.rochester.edu/mth/sites/doug-ravenel/mybooks/ravenel.pdf">The Green Book</a>, Doug Ravenel. Chapter 3 has some classic Adams spectral sequence computations.
    </li>
    <li>[The Adams spectral sequence and Hopf algebroids](/files/The_Adams_spectral_sequence_and_Hopf_algebroids%20(2).pdf), Jackson Morris. This is a short write up I made which sets up the Adams spectral sequence from the point of view of affine groups schemes and Hopf algebroids.
    </li>
    </ul>
    </details>

<!-- * **Adams-Novikov Spectral Sequence**

* **Algebraic Novikov Spectral Sequence**

* **Atiyah-Hirzebruch Spectral Sequence**

* **Bar spectral Sequence** -->

* **$\text{bo}$-resolution**
    <details>
    <summary>See more</summary>
    The bo-resolution is the bo-based Adams spectral sequence.
    <ul>
    <li> <a href= "https://projecteuclid.org/journals/pacific-journal-of-mathematics/volume-92/issue-2/brm-o-resolutions/pjm/1102736799.full">bo-resolutions</a>, Mark Mahowald. Mahowald studies the bo-resolution for the first time in this paper. He uses the spectral sequence to compute the 2-primary v1-periodic stable homotopy groups of spheres. the results are later used, or suitably interpreted here, to prove the height 1 telescope conjecture at the prime 2.
    </li>
    </ul>
    </details>

* **Bockstein Spectral Sequence**

* **Bokstedt Spectral Sequence**
    <details>
    <summary>See more</summary>
    The Bokstedt spectral sequence is a tool for computing the homology of the THH of a ring.
    <ul>
    <li> <a href ="https://arxiv.org/pdf/math/0502195">Hopf Algebra Structures on Topological Hochschild Homology</a>, Vigeik Angeltveit and John Rognes. A terrific paper to read if you want to start getting your hands dirty with computations using the Bokstedt spectral sequence in the context of chromatic homotopy theory, redshift, the Adams spectral sequence, etc.
    </li>
    <li> <a href ="https://arxiv.org/abs/1705.03343">The Segal Conjecture for Topological Hochschild Homology of the Ravenel Spectra</a>, Gabe Angelini-Knoll and J.D. Quigley. Short, sweet, and to the point. Computes THH of X(n) and T(n) by the Bokstedt spectral sequence.
    </li>
    <li> <a href ="https://arxiv.org/abs/1908.09164">A Homological Approach to Chromatic Complexity of Algebraic K-theory</a>, Gabe Angelini-Knoll and J.D. Quigley. Computes THH of y(n) by the Bokstedt spectral sequence.
    </li>
    <li> <a href="https://arxiv.org/abs/1906.03057">The Topological Hochschild Homology of the Algebraic K-theory of Finite Fields</a>, Eva Honing. Compute THH of the algebraic K-theory of the finite fields by the Boksted spectral sequence.
    </li>
    <li> <a href="https://www.davidmehrle.com/notes/references/bokstedt2.pdf">The Topological Hochschild Homology of Z and Z/p</a>, Marcel Bokstedt. Origin of the Bokstedt spectral sequence.
    </li>
    </ul>
    </details>

* **Bousfield-Kan Spectral Sequence**

* **Cartan-Eilenberg Spectral Sequence**

* **Chromatic Spectral Sequence**
    <details>
    <summary>See more</summary>
    The chromatic spectral sequence is a spectral sequence converging to the E2-term of the Adams-Novikov spectral sequence.
    <ul>
    <li> <a href = "https://math.mit.edu/events/talbot/2013/3-Rasekh-CSS.pdf">The chromatic spectral sequence</a>, Nima Rasekh. Short set of notes from 2013 Talbot. </li>
    <li> <a href = "https://drive.google.com/file/d/14DIYf2v4zhEUuZSsZcbYBwjyoeyL21r4/view">Spectral Sequences from Sequences of Spectra: Towards the Spectrum of the Category of Spectra</a>, Dylan Wilson. Great set of notes, chapter 2 covering the chromatic spectral sequence. </li>
    <li> <a href = "https://www.sas.rochester.edu/mth/sites/doug-ravenel/mypapers/mrw.pdf">Periodic phenomena in the Adams-Novikov Spectral Sequence</a>, Haynes Miller, Doug Ravenel, and W. Stephen Wilson. The origin story. </li>
    <li> <a href = "https://www.ams.org/journals/tran/1987-300-01/S0002-9947-1987-0871672-0/">Periodic phenomena in the classical Adams spectral sequence</a>, Mark Mahowald and Paul Schick. This paper asks and answers its title question. </li>
    <li> <a href ="https://www.ams.org/journals/tran/1987-300-01/S0002-9947-1987-0871672-0/">The homotopy groups \pi_*(L_2 S^0) at the prime 3</a>, Katsumi Shimomura and Xiangjunn Wang. An actual computation with the chromatic spectral sequence! </li>
    </ul>
    </details>
* **Descent Spectral Sequence**

* **Double Complex Spectral Sequence**

* **EHP Spectral Sequence**

* **Eilenberg-Moore Spectral Sequence**

* **Filtration Spectral Sequence**

* **Goodwillie Spectral Sequence**

* **Grothendieck Spectral Sequence**

* **Homotopy Fixed Point Spectral Sequence**

* **$\text{kq}$-resolution**
    <details>
    <summary>See more</summary>
    The kq-resolution is the kq-based motivic Adams spectral sequence.
    <ul>
    <li> <a href = "https://arxiv.org/abs/1905.11952">kq-resolutions I</a>, Dominic Culver and J.D. Quigley. Computes the C-motivic kq resolution, determining the v1-periodic stable stems. </li>
    <li> <a href ="https://arxiv.org/abs/2506.16672">On the Ring of Cooperations for Real Hermitian K-theory</a>, Jackson Morris. I determined the E1-page of the kq-resolution over the real numbers. </li>
    <li> <a href ="https://arxiv.org/abs/2509.02786">Rings of Cooperations for Hermitian K-theory over Finite Fields</a>, Jackson Morris. I determined the E1-page of the kq-resolution over all finite fields of characteristic different from 2. </li>
    </ul>
    </details>

* **Kunneth Spectral Sequence**

* **Localized Adams Spectral Sequence**

* **Lyndon-Hochschild-Serre Spectral Sequence**

* **May Spectral Sequence**

* **Motivic Spectral Sequence**

* **Relative Adams Spectral Sequence**

* **Serre Spectral Sequence**

* **Slice Spectral Sequence**

* **$\text{tmf}$-resolution**
    <details>
    <summary>See more</summary>
    The tmf-resolution is the tmf-based Adams spectral sequence.
    <ul>
    <li> <a href = "https://arxiv.org/abs/1909.13379">The Telescope Conjecture at Height 2 and the tmf-resolution</a>, Agnes Beaudry, Mark Behrens, Prasit Bhattacharya, Dominic Culver, and Zhouli Xu. An attempt to lift Mahowald's use of the bo-resolution and his study of height 1 chromatic phenomena to the height 2 world.
    </li>
    </ul>
    </details>

* **Tate Spectral Sequence**

* **Universal Coefficient Spectral Sequence**

* **Unstable Adams Spectral Sequence** 
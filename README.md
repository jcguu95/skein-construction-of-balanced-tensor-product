# Compilation

Structure is given in `main.tex`.

To make the document, run `$ make`.

# TODOs

### 1. Prove that sk(M,C,N) is abelian.

This is a significant gap in our work. Manuel noted that there exists an
alternative definition of a k-linear category. However, we are using Douglas's
definition, which requires the category to be abelian. Consequently, we must
establish that our model sk(M,C,N) is abelian before proving that it satisfies
the universal property. In the current version, Jin overlooked this
requirement and incorrectly asserted its abelian property as a corollary.

There are three possible ways to prove it.

+ (a) Prove it directly, which will be tedious.

+ (b) Use theorems related to Karoubi completion to conclude that Kar(X) is
  abelian, assuming X meets certain conditions. The issue is that Jin is not
  aware of any theorems supporting this conclusion. It appears to be
  established that Karoubi completion is always "pseudo-abelian" [1], which is
  a strictly weaker property than "abelian" [1].

+ (c) (Idea from Manuel): Demonstrate that a specific hom-space algebra is a
  finite-dimensional semisimple algebra. We have finite dimensionality,
  supported by Jin's basis theorem already, so what's remaining is
  semisimplicity. Manuel mentioned that this parallels a proof by Thibault
  Décoppet in an easier case.

However, Jin believes this approach (c) could prove very challenging, as it
closely approaches the process of semisimplifying a finite-dimensional algebra
with given structural coefficients. This is nearly as difficult as providing a
constructive proof of the Artin-Wedderburn theorem. While Jin is not an expert
in this area, his research suggests that it's quite challenging. Successfully
completing this would be a breakthrough, as it would enable the computation of
the simples of the Drinfeld center, in particular. The most recent progress in
this direction was published this summer [2], presenting a probabilistic
algorithm; however, the paper notes that it is not yet efficient enough to
compute anything new. This algorithm relies on the Meat-Axe algorithm, which
is well-introduced in [3].

### 2. Deal with right-exactness.

This part should not be difficult, as we assume semisimplicity.

### 3. Comment on Deligne vs Kelly Tensor Product.

To relax our assumptions (finite and semisimple), challenges emerge when
taking the Deligne tensor product in the early stages of our construction. In
order to generalize in that direction, one may have to change the definition
of the balanced tensor product that incorporates Kelly tensor product, which
is known to generalize Deligne tensor product [4].

Manuel will add a casual remark on this, aimed at helping those interested in
future generalizations of the work.

### 4. Manuel's clever proof for Main Lemma.

Manuel has come up with another clever and insightful proof for the main
lemma, breaking down the steps and utilizing several established theorems. He
will add it to the construction section, and Jin will integrate it into the text
soon.

### 5. Jin clarifies with T Gannon applications to VOA.

### (Small) Just use "retracts" instead of subobjects throughout.

\eta*(1_{\boxtimes_C}:=\eta_{\boxtimes_C}

horizontal composition \circ_h

### Explain how a direct proof for abelian+semisimple could be done

Add a remark citing (2.5.5 of Dualizable Tensor Categories) that their direct
proof for separability (in particular, abelian and semisimple) should be
translatable into our context.

### Integrate Manuel's work

And resolve the following points.

[suggestion] Make a begin/proof section for proposition 1.13. And add
reference numbers to the "following three lemmas".

[suggestion] In the proof of lemma 2.16, I think I would stress that we will
just prove "abelianity" instead of "k-linear", as the difference is trivial to
prove. Therefore we show that every morphism has a kernel (and by the dual
argument it also has a cokernel).

[suggestion] Say explicitly that sk(M,C,N) is "k-linear" finite semisimple.
Then in the proof of 2.19, we can just say sk(M,C,N) is a k-linear finite
semisimple (and in particular abelian). I think it's also better to move that
first line in proof 2.19 to the second final line, and add "among the k-linear
categories" after "the defining universal property". Finally, add a reference
for the universal property.

[suggestion] In remark 2.20, I think it's worth saying that [DSS20] contains
results that work for general fields. In particular.. [enter what you had].
And add "this may help extension of this work to more general conditions in
the future", to clarify the intention of this remark.

[gap] In the proof of proposition 2.17. This was where I got stuck last week.
More precisely, "finite" got me stuck. In [EGNO, def 1.8.6], the definition of
"finite" includes "having enough projectives", i.e. each object has to have a
projective cover. As M \subset N, any m has a projective cover in N. We need
to argue why that cover can be altered to be in M.

# Reference

+ [1] [Karoubi envelope in
  nLab](https://ncatlab.org/nlab/show/Karoubi+envelope)
+ [2] [[2406.13438] Computing the center of a fusion
  category](https://arxiv.org/abs/2406.13438)
+ [3] Representations of groups - A computational approach-[Klaus Lux, Herbert
  Pahlings]
+ [4] Work of Ignacio López Franco

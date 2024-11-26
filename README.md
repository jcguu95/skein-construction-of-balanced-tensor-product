# Compilation

Structure is given in `main.tex`.

To make the document, run `$ make`.

# TODOs

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

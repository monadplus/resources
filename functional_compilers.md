Resources on Compilers for Functional Languages
===============================================


These courses follow [An Incremental Approach to Compiler Construction -  A. Ghuloum](http://scheme2006.cs.uchicago.edu/11-ghuloum.pdf) (written in Scheme) while building a compiler from a functional language to x86/C wrapper:

- http://www.ccs.neu.edu/course/cs4410/ - written in OCaml
- [Essentials of Compilation](https://jeapostrophe.github.io/courses/2017/spring/406/notes/book.pdf) - written in Racket - book format

And another course covering the _intermediate_ stage of compiling functional languages:
- [Compiling Functional Languages](http://www.cse.chalmers.se/edu/year/2011/course/CompFun/)

### Books

- Modern Compiler Implementation in ML - Andrew W. Appel

### Short Overviews

- [Haskell and Compilers](https://github.com/soupi/rfc/blob/master/compilers-and-haskell.md)
- [Compiling Lisp to JavaScript from Scratch in 350 LOC](https://gilmi.me/blog/post/2016/10/14/lisp-to-js)
- [elaboration-zoo](https://github.com/AndrasKovacs/elaboration-zoo) - Repo with the following topics written in Haskell: evaluation of HOAS and closures, type-checking, holes, implicit arguments.

### Parsing

- [Grammars - The Language of Languages](http://matt.might.net/articles/grammars-bnf-ebnf/)
- [Type Classes - Parsing](https://typeclasses.com/parsing) (Haskell)
- [Intro to Parsing with Parsec in Haskell](https://jakewheat.github.io/intro_to_parsing/)

#### Tools

- [Backus-Naur Form Converter](https://bnfc.readthedocs.io/en/latest/) - generates a lexer and parser from a BNF specification of your grammar. It has several destination languages (Haskell, Java, etc)

### Type-checking

- [Simon Peyton Jones - how GHC type inference engine actually works](https://www.youtube.com/watch?v=x3evzO8O9e8)
- [Type Inference (PAPL)](https://papl.cs.brown.edu/2020/Type_Inference.html)
- [The Essence of ML Type Inference](http://gallium.inria.fr/~fpottier/publis/emlti-final.pdf)
- [Correcting A Widespread Error in Unification Algorithms](http://norvig.com/unify-bug.pdf)
- [Generalizing Hindley-Milner Type Inference Algorithms](http://soft.vub.ac.be/~cfscholl/Capita-Selecta-2015/papers/2002%20Heeren.pdf)
- [Typing Haskell in Haskell](https://gist.github.com/chrisdone/0075a16b32bfd4f62b7b)

#### Type Theory

- [Types and Programming Languages - Benjamin C. Pierce](https://www.cis.upenn.edu/~bcpierce/tapl/)

### Rewrites

- [A-Normalization](http://matt.might.net/articles/a-normalization/)
- [Building Small Native Languages with Haskell](http://dev.stephendiehl.com/paris.pdf)

#### Inlining

- [Secrets of the GHC inliner](https://www.microsoft.com/en-us/research/wp-content/uploads/2002/07/inline.pdf)


### Runtime Systems

- [CHICKEN data representation](http://www.more-magic.net/posts/internals-data-representation.html)
- [Automated Memory Management (Overview)](https://papl.cs.brown.edu/2013/Automated_Memory_Management.html)
- [Baby's First Garbage Collector](http://journal.stuffwithstuff.com/2013/12/08/babys-first-garbage-collector/)
- [CHICKEN Scheme's garbage collector](http://www.more-magic.net/posts/internals-gc.html)
- [CEK Machines](http://matt.might.net/articles/cek-machines/)
- [CESK Machines](http://matt.might.net/articles/cesk-machines/)
- [The ZINC Experiment](http://caml.inria.fr/pub/papers/xleroy-zinc.pdf)
- [Implementing lazy functional languages on stock hardware: The Spineless Tagless G-Machine](https://www.microsoft.com/en-us/research/wp-content/uploads/1992/04/spineless-tagless-gmachine.pdf)
- [Compiler Design: Virtual Machine](http://www.springer.com/gp/book/9783642149085)

### Refinement Types

- [An tutorial-style implementation of liquid/refinement types for a subset of Ocaml/Reason](https://github.com/ranjitjhala/sprite-lang)

Resources on low-level Haskell
==============================

- [GHC development](https://ghc.dev/)
- [I know kung fu: learning STG by example](https://gitlab.haskell.org/ghc/ghc/-/wikis/commentary/compiler/generated-code)
- [Levity polymorphism](https://downloads.haskell.org/~ghc/latest/docs/html/users_guide/glasgow_exts.html#levity-polymorphism)
- [Calling Haskell from C](https://wiki.haskell.org/Calling_Haskell_from_C)
- [Purpose of memory alignment](https://stackoverflow.com/questions/381244/purpose-of-memory-alignment)
- [Delimited continuation primops](https://github.com/ghc-proposals/ghc-proposals/pull/313)
- [Inlining and Specialisation](https://wiki.haskell.org/Inlining_and_Specialisation)

### Where to start

- https://www.aosabook.org/en/ghc.html
- https://www.haskell.org/onlinereport/haskell2010/haskellpa1.html#haskellch2.html
- https://www.stephendiehl.com/posts/ghc_01.html
- https://gitlab.haskell.org/ghc/ghc/-/wikis/reading-list
- A

### Core

- [A transformation-based optimiser for Haskell](https://www.microsoft.com/en-us/research/wp-content/uploads/1998/09/comp-by-trans-scp.pdf)

- http://smart-cactus.org/~ben/posts/2015-01-19-understanding-ghc-core.html
- https://gitlab.haskell.org/ghc/ghc/-/wikis/commentary/compiler/core-syn-type
- https://gitlab.haskell.org/ghc/ghc/blob/master/compiler/GHC/Core.hs#L326

### Libraries

- [GHC.Exts](https://hackage.haskell.org/package/base-4.12.0.0/docs/GHC-Exts.html)
- [ghc-prim](https://hackage.haskell.org/package/ghc-prim) - GHC primitives
- [primitive](https://hackage.haskell.org/package/primitive-0.7.0.1) - primitive memory-related operations
- [array](https://hackage.haskell.org/package/array)
- [vector](https://hackage.haskell.org/package/vector)
- [ghc-core](http://hackage.haskell.org/package/ghc-core) - Display GHC's core and assembly output in a pager

Resources on Haskell
====================

- [List of foundational resources](https://github.com/cohomolo-gy/haskell-resources)
- [List of optics resources](https://github.com/cohomolo-gy/optics-resources), [Optics: cheatsheet](https://gist.github.com/monadplus/4c742bd49ff601ad1dd49f4dcac9c5e3)
- [State of the Haskell ecosystem](https://github.com/Gabriel439/post-rfc/blob/master/sotu.md)
- [What I Wish I Knew When Learning Haskell](http://dev.stephendiehl.com/hask/index.html)
- [Simple Haskell](https://www.simplehaskell.org/)
- [Agda vs. Coq vs. Idris](https://whatisrt.github.io/dependent-types/2020/02/18/agda-vs-coq-vs-idris.html) - Comparison between languages
- [Can someone explain to me the benefits of IO?](https://www.reddit.com/r/scala/comments/8ygjcq/can_someone_explain_to_me_the_benefits_of_io/e2jfp9b/)
- [Type-classes are nothing like interfaces](https://blog.tmorris.net/posts/type-classes-are-nothing-like-interfaces/index.html)
- [Liquid Haskell](https://ucsd-progsys.github.io/liquidhaskell/), [Implementing a GHC Plugin for Liquid Haskell](https://www.well-typed.com/blog/2020/08/implementing-a-ghc-plugin-for-liquid-haskell/)
- [A list of every data exchange formats I could find](https://gist.github.com/gelisam/13d04ac5a54b577b2492785c1084281f) - swagger, json-schema, avro, thrift, capt'n proto, asn.1 ...
- [Beatinc C With 80 Lines of Haskell: wc](https://chrispenner.ca/posts/wc)
- [How does haskell make your life easier?](https://williamyaoh.com/posts/2019-11-30-how-does-haskell-make-life-easier.html)
- [Region-based resource management](http://okmij.org/ftp/Haskell/regions.html)
- [API desin](https://gist.github.com/Gabriel439/563fa662f84e0a845c79775756cfce78)
- [The three kinds of haskell exceptions and how to use them](https://www.tweag.io/blog/2020-04-16-exceptions-in-haskell/)
- [bracketing and async exceptions in haskell](https://joeyh.name/blog/entry/bracketing_and_async_exceptions_in_haskell/) - bracket can still fail!
- [foldl vs. foldr](https://github.com/hasura/graphql-engine/pull/2933#discussion_r328821960) - well explained
- [What does Haskell do better than Scala](https://www.reddit.com/r/hascalator/comments/ahv098/ok_ill_bite_what_does_haskell_do_better_than_scala/eeocdhl/)
- [oneShot](https://hackage.haskell.org/package/base-4.14.0.0/docs/GHC-Exts.html#v:oneShot) - The oneShot function can be used to give a hint to the compiler that its argument will be called at most once, which may (or may not) enable certain optimizations. It can be useful to improve the performance of code in continuation passing style.
- [How haskell threads block](http://www.wjwh.eu/posts/2020-07-10-haskell-thread-blocked.html)
- [Template Haskell: staging](http://web.cecs.pdx.edu/~sheard/course/AdvancedFP/notes/StagingInHaskell.pdf)
- [Functionally oblivious (and succinct)](https://www.cs.ox.ac.uk/ralf.hinze/WG2.8/33/slides/Edward.pdf)
- [Cache-friendly binary search](http://bannalia.blogspot.com/2015/06/cache-friendly-binary-search.html)
- [Library: jsonifier](https://github.com/nikita-volkov/jsonifier) - x3 faster than Aeson by preallocating a buffer of the size of the resulting marshalling

### Clever Haskell

- [Random Access Lists](https://doisinkidney.com/posts/2020-05-02-more-random-access-lists.html)
- [type (~Ꭱ) = Coercible](https://www.reddit.com/r/haskelltil/comments/dh9z2a/type_coercible/)
- [Opaque Constraint Synonyms](https://kcsongor.github.io/opaque-constraint-synonyms/)
- [Replacing function arguments with MonadReader calls](https://gist.github.com/i-am-tom/23d36a0598936572407794883548c900)
- [Typerep-map step by step](https://kowainik.github.io/posts/2018-07-11-typerep-map-step-by-step)
- [Higher-Kinded Data](https://reasonablypolymorphic.com/blog/higher-kinded-data/)
- [Deriving Bifunctor with Generics](https://kcsongor.github.io/generic-deriving-bifunctor/#incoherent-instances)
- [Session Types: workshop](https://github.com/coot/monadic-party2019)
- [Parsing type-level strings in Haskell](https://kcsongor.github.io/symbol-parsing-haskell/)

### Laziness & Space Leaks

- [Laziness Quiz](https://www.parsonsmatt.org/2018/12/04/laziness_quiz.html)
- [Spaceleak detection](https://github.com/ndmitchell/spaceleak) - How to blog (recommended)
- [Destroying Performance with Strictness](https://neilmitchell.blogspot.com/2013/08/destroying-performance-with-strictness.html)
- [Time travel in Haskell for dummies](https://kcsongor.github.io/time-travel-in-haskell-for-dummies/) - laziness in action. Very cool post.

### Databases

- [Which type-safe database library should you use?](https://williamyaoh.com/posts/2019-12-14-typesafe-db-libraries.html)
- [Database testing](https://gist.github.com/monadplus/862d130ccd9a959581e00bf8e99b47f4)

### Data Science

- [Current Environment](http://www.datahaskell.org/docs//community/current-environment.html)

### Build Tools

- [Most popular build tools](./haskell/build_tools.md)

### Package Versioning Policy (PVP)

- [Haskell PAckage Versioning Policy](https://pvp.haskell.org/?rdfrom=https%3A%2F%2Fwiki.haskell.org%2Findex.php%3Ftitle%3DPackage_versioning_policy%26redirect%3Dno)
- [On PVP and Restrictive Bounds](https://www.reddit.com/r/haskell/comments/gf7uw8/on_pvp_and_restrictive_bounds/fpv3dtg/)
- [Hackage Metadata Revisions — What They Are, How They Work](https://github.com/haskell-infra/hackage-trustees/blob/master/revisions-information.md)

### Libraries

- [Most popular libraries by topic](./haskell/libraries.md)

### Design Patterns:

- [The Service Pattern](https://www.schoolofhaskell.com/user/meiersi/the-service-pattern)
- [The Handle Pattern](https://jaspervdj.be/posts/2018-03-08-handle-pattern.html)

### GHC & System/Low-level Programming

- [The GHC: a contributor's cheatsheet](https://ghc.dev/)
- [About GHC & System Programming in Haskell](./haskell/low_level.md)
- [A short exploration of GHC’s instance resolution hiding mistakes from the type checker](https://dorchard.blog/2020/06/03/a-short-exploration-of-ghcs-instance-resolution-hiding-mistakes-from-the-type-checker/) - Instance resolution prevented a typechecking error explained
- [Better instance resolution error](https://mgsloan.com/posts/inspecting-haskell-instance-resolution/) - About adding a new flag to GHC to "explain" instances resolution
- [GHC version - base version](https://wiki.haskell.org/Base_package)

### Effect Systems

- [Most popular effect systems](./haskell/effect-systems.md)

### Editors/IDEs

- [Most popular editors/ide](./haskell/editors.md)

### CI Tools

- [Dead simple cross-platform GitHub Actions for Haskell](https://kodimensional.dev/github-actions)
- [GitHub actions for Haskell CI](https://markkarpov.com/post/github-actions-for-haskell-ci.html)

### Nix

- [Nix and Haskell in production](https://github.com/Gabriel439/haskell-nix) - How to develop and build your haskell applications using Nix (recommended)
- [Nix Haskell Monorepo Tutorial](https://github.com/fghibellini/nix-haskell-monorepo)

- More about nix [here](./nix.md)

### Exercises

- [Advent of Code](https://adventofcode.com/)
- [Kattis](https://open.kattis.com/)

### Blogs

- [Csongor Kiss](https://kcsongor.github.io/)
- [Sandy Maguire](https://reasonablypolymorphic.com/)
- [Johan Tibell](http://blog.johantibell.com/)
- [Oleg Kiselyov](http://okmij.org/ftp/)
- [Dmitrii Kovanikov](https://kodimensional.dev/)
- [Kowainik](https://kowainik.github.io/)
- [Joachim Breitner](https://www.joachim-breitner.de/blog)
- [Colin Woodbury (Fosskers)](https://www.fosskers.ca/en/blog)

### Books

- Haskell from first principles - Allen and Moronuki
- Parallel and Concurrent Programming in Haskell - Simon Marlow
- [Algebra-Driven Design - Sandy Maguire](https://algebradriven.design/)
- Thinking With Types - Sandy Maguire
- Algorithm Design With Haskell - Bird and Gibbons
- [Functional Design and Architecture - Alexander Granin](https://graninas.com/functional-design-and-architecture-book/)

### Conferences

- [Monadic Party](https://monadic.party/)
- Zurihack
- Lambda Days
- [Haskell Love Conference](https://haskell.love/)
- [ICFP](https://icfp20.sigplan.org/)

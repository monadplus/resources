# Resources on Haskell Libraries

- [deepseq](https://hackage.haskell.org/package/deepseq)
- [flux-monoid](http://hackage.haskell.org/package/flux-monoid) - A monoid for tracking changes
- [monoidal-containers](http://hackage.haskell.org/package/monoidal-containers) - containers with merging via monoid
- [mono-traversable](https://hackage.haskell.org/package/mono-traversable) - mono-traversable: Type classes for mapping, folding, and traversing monomorphic containers
- [vector-builder](https://hackage.haskell.org/package/vector-builder)
- [stream-fusion](https://hackage.haskell.org/package/stream-fusion) - faster haskell lists using stream fusion
- [monad-control](https://hackage.haskell.org/package/monad-control) - Lift control operations, like exception catching, through monad transformers
- [unliftio](https://hackage.haskell.org/package/unliftio) - try to implement `withBinaryFile :: FilePath -> IOMode -> (Handle -> IO a) -> IO a` using `MonadIO`
- [safe-exceptions](https://hackage.haskell.org/package/safe-exceptions)
- [base-compat](https://hackage.haskell.org/package/base-compat) - Provides functions available in later versions of base to a wider range of compilers
- [typerep-map](https://github.com/kowainik/typerep-map) - Keys as values' types
- [haskell-src-exts](https://hackage.haskell.org/package/haskell-src-exts) - Manipulating Haskell source: abstract syntax, lexer, parser, and pretty-printer
- [neat-interpolation](https://hackage.haskell.org/package/neat-interpolation) - A quasiquoter for neat and simple multiline text interpolation
- [recursion-schemes](https://hackage.haskell.org/package/recursion-schemes)
- [algebraic-graphs](https://hackage.haskell.org/package/algebraic-graphs)
- [directory](https://hackage.haskell.org/package/directory)
- [hashable](https://hackage.haskell.org/package/hashable)
- [constraints](https://hackage.haskell.org/package/constraints) - Vocabulary for working with constraints.
- [show-combinators](https://hackage.haskell.org/package/show-combinators) - combinators to write Show instances.
- [tuple-morph](https://hackage.haskell.org/package/tuple-morph-0.1.0.0) - morphism between tuples

## Custom Preludes

- [relude](https://hackage.haskell.org/package/relude)
- [protolude](https://hackage.haskell.org/package/protolude)
- [rio](https://hackage.haskell.org/package/rio)

## Web Framework

- [servant](https://hackage.haskell.org/package/servant-server)
- [scotty](https://hackage.haskell.org/package/scotty)
- [yesod](https://hackage.haskell.org/package/yesod)
- [snap](https://hackage.haskell.org/package/snap-server)

### HTTP Client

- [servant-client](https://hackage.haskell.org/package/servant-client)
- [req](https://hackage.haskell.org/package/req)

### Front end

- [miso](https://github.com/dmjio/miso)
- [miso template example](https://github.com/serras/miso-start-template)

#### HTML

- [blaze-html](http://hackage.haskell.org/package/blaze-html) - HTML combinator library
- [lucid](http://hackage.haskell.org/package/lucid) - HTML combinator library

- [Choosing an HTML library in Haskell](https://vrom911.github.io/blog/html-libraries)

#### CSS

- [clay](https://hackage.haskell.org/package/clay) - CSS preprocessor as embedded Haskell

## Error & Error Handling

- [plucky](https://hackage.haskell.org/package/plucky-0.0.0.1/docs/Data-Either-Plucky.html)

- [prio](https://github.com/parsonsmatt/prio/blob/master/src/Lib.hs) - Errors properly encoded on types (snippet).

## Parallelism & Concurrency

Parallelism:

- [parallel](https://hackage.haskell.org/package/parallel)
- [monad-par](https://hackage.haskell.org/package/monad-par)
- [accelerate](https://hackage.haskell.org/package/accelerate)

Concurrency:

- [async](https://hackage.haskell.org/package/async), [lifted-async](https://hackage.haskell.org/package/lifted-async)
- [concurrency](https://hackage.haskell.org/package/concurrency) - A typeclass abstraction over much of Control.Concurrent

## Type-level Programming

- [singletons](https://hackage.haskell.org/package/singletons) - framework for generating singleton types
- [symbols](https://hackage.haskell.org/package/symbols) - symbol manipulation
- [decidable](http://hackage.haskell.org/package/decidable) - Type-level predicates: k ~> Type. Complementary to singletons.

- [ghc-typelits-natnormalise](https://hackage.haskell.org/package/ghc-typelits-natnormalise) - GHC typechecker plugin for types of kind GHC.TypeLits.Nat
- [ghc-typelits-knownnat](https://hackage.haskell.org/package/ghc-typelits-knownnat) - Derive KnownNat constraints from other KnownNat constraints
- [typelevel-rewrite-rules](https://hackage.haskell.org/package/typelevel-rewrite-rules)

## Streaming

- [conduit](https://hackage.haskell.org/package/conduit)
- [pipes](http://hackage.haskell.org/package/pipes)
- [streaming](https://hackage.haskell.org/package/streaming)
- [io-streams](https://hackage.haskell.org/package/io-streams)
- [iteratee](https://hackage.haskell.org/package/iteratee)
- [enumerator](https://hackage.haskell.org/package/enumerator)
- [foldl](https://hackage.haskell.org/package/foldl)

## Parsing

- [parsec](https://hackage.haskell.org/package/parsec)
- [attoparsec](https://hackage.haskell.org/package/parsec) - bulk parsing of large text and binary files instead of parsing language syntax to ASTs ([efficient](http://www.serpentine.com/blog/2014/05/31/attoparsec/)
- [parsec vs attoparsec](https://stackoverflow.com/questions/19208231/attoparsec-or-parsec-in-haskell/19213247#19213247)
- [megaparsec](https://hackage.haskell.org/package/megaparsec) - generalisation and optimisation of  parsec
- [trifecta](https://hackage.haskell.org/package/trifecta)
- [Earley](https://hackage.haskell.org/package/Earley) - parsing all context-free grammars using Earley's algorithm

## Serialisation

### Binary

- [binary](https://hackage.haskell.org/package/binary)
- [cereal](https://hackage.haskell.org/package/cereal)
- [flat](https://hackage.haskell.org/package/flat)
- [binary vs cereal](https://stackoverflow.com/questions/14658031/cereal-versus-binary)
- [serialisation libraries benchmarks](https://github.com/haskell-perf/serialization)

### CSV

- [cassava](https://hackage.haskell.org/package/cassava)

### JSON

- [aeson](https://hackage.haskell.org/package/aeson), [aeson-qq](https://hackage.haskell.org/package/aeson-qq), [aeson-pretty](https://hackage.haskell.org/package/aeson-pretty)
- [jsonifier](https://github.com/nikita-volkov/jsonifier) - x3 faster than Aeson by preallocating a buffer of the size of the resulting marshalling
- [deriving-aeson](https://hackage.haskell.org/package/deriving-aeson)

### Version numbers

- [versions](https://hackage.haskell.org/package/versions)

## Data Structures

- [structures](https://hackage.haskell.org/package/structures) - advanced data structures
- [psqueues](https://hackage.haskell.org/package/psqueues) - priority search queues
- [bloomfilter](https://github.com/bos/bloomfilter)
- [treap](https://github.com/chshersh/treap) - Implicit treap

## Logging

- [co-log](https://hackage.haskell.org/package/co-log)
- [fast-logger](https://hackage.haskell.org/package/fast-logger)
- [monad-logger](https://hackage.haskell.org/package/monad-logger)

## Databases

- [hasql](https://hackage.haskell.org/package/hasql), [hasql-transaction](https://hackage.haskell.org/package/hasql-transaction), [hasql-pool](https://hackage.haskell.org/package/hasql-pool) - PostgreSQL
- [persistent](https://hackage.haskell.org/package/persistent)

## Lens

- [lens](https://hackage.haskell.org/package/lens), [lens-aeson](https://hackage.haskell.org/package/lens-aeson]), [lens-action](https://hackage.haskell.org/package/lens-action), [lens-regex-pcre](https://hackage.haskell.org/package/lens-regex-pcre), [lens-csv](https://hackage.haskell.org/package/lens-csv), [generic-lens](https://hackage.haskell.org/package/generic-lens)
- [microlens](https://hackage.haskell.org/package/microlens), microlens-platform
- [generic-lens](https://hackage.haskell.org/package/generic-lens) - A piece of art


## Command-line / Terminal

- [optparse-applicative](https://hackage.haskell.org/package/optparse-applicative)
- [optparse-generic](https://hackage.haskell.org/package/optparse-generic)
- [colourista](https://github.com/kowainik/colourista) - colored messages in the terminal
- [haskeline](https://hackage.haskell.org/package/haskeline) - Interactive (InputT m a)

## Regex

- [pcre-light](https://hackage.haskell.org/package/pcre-light)

## Random Number Generators

- [mwc-random](https://hackage.haskell.org/package/mwc-random) - Has several distributions implemented

## Graphics

- [chart](https://hackage.haskell.org/package/Chart), [chart-diagrams](https://hackage.haskell.org/package/Chart-diagrams) - 2D charts and plots
- [gloss](https://hackage.haskell.org/package/gloss) - 2D vectorial graphics
- [brick](https://hackage.haskell.org/package/brick) - Terminal User Interface (TUI) toolkit

## Shell & processes

- [turtle](https://hackage.haskell.org/package/turtle) - shell scripting
- [typed-process](https://hackage.haskell.org/package/typed-process) - run external processes, with strong typing of streams

## Cabal

- [packunused](http://hackage.haskell.org/package/packunused) - detect redundant Cabal package dependencies

## Distributed Computation

- [distributed-process](https://hackage.haskell.org/package/distributed-process)

## Currencies

- [safe-money](https://hackage.haskell.org/package/safe-money) - type-safe and lossless encoding and manipulation of money.

## Time

- [A Haskell Time Library Tutorial](https://two-wrongs.com/haskell-time-library-tutorial)
- [chronos](https://hackage.haskell.org/package/chronos) - performant time library

## Testing

- [inspection-testing](http://hackage.haskell.org/package/inspection-testing) - GHC plugin to compare producted Core
- [generic-random](https://hackage.haskell.org/package/generic-random) - Generic random generators for QuickCheck
- [doctest](https://hackage.haskell.org/package/doctest) - test examples in source code comments

- [QuickCheck](https://hackage.haskell.org/package/QuickCheck), [The Design and Use of QuickCheck](https://begriffs.com/posts/2017-01-14-design-use-quickcheck.html)
- [hedgehod](https://hackage.haskell.org/package/hedgehog)

- [QuickSpec](https://hackage.haskell.org/package/quickspec) - discover equational laws for free

## FFI

- [hsc2hs](https://hackage.haskell.org/package/hsc2hs) - A preprocessor that helps with writing Haskell bindings to C code
- [parle](https://gitlab.com/chrisdone-fp/parle) - Call Rust from Haskell, simple example.

## TH

- [template-haskell](https://hackage.haskell.org/package/template-haskell)
- [th-abstraction](https://hackage.haskell.org/package/th-abstraction) - reified information about data types

## Networking

- [network](https://hackage.haskell.org/package/network)

## Monitoring

- [ekg](https://hackage.haskell.org/package/ekg) - remote monitoring of processes

## Benchmark

- [criterion](https://hackage.haskell.org/package/criterion)
- [gauge](https://hackage.haskell.org/package/gauge) - small framework for performance measurement

## Effect Systems

- [Here](./effect-systems.md)

## Combinatorial Problem

### Constraint Programming

- [holmes](https://hackage.haskell.org/package/holmes) - Constraint Programming

### Integer Linear Programming (ILP)

- [limp-cbc](https://hackage.haskell.org/package/limp-cbc)

### SAT

- [toysolver](https://hackage.haskell.org/package/toysolver)

### Hardware

- [clash lang](https://clash-lang.org/)

## Others

- [haxl](https://hackage.haskell.org/package/haxl) - simplifies access to remote data, such as databases or web-based services
- [hpack](https://github.com/sol/hpack#readme) - A modern format for Haskell packages
-[ghc-musl](https://github.com/utdemir/ghc-musl) - Fully Static Haskell binaries without glibc dependency on any platform which can run Docker.
- [hint](https://hackage.haskell.org/package/hint) - haskell interpreter as a library

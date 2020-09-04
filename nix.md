Resources on Nix
================

- [Nix Package Manager](https://nixos.org/manual/nix/stable/)
- [NixOS](https://nixos.org/manual/nixos/stable/)
- [Nixpkgs](https://nixos.org/manual/nixpkgs/stable/)
- [Hydra](https://github.com/NixOS/hydra) - CI tool for Nix

### Commands

Main commands:

- `nix-env`
- `nix-build`
- `nix-shell`
- `nix-store`

Utilities:

- `nix-serve`
- `nix-channel`
- `nix-collect-garbage`
- `nix-copy-closure`
- `nix-daemon`
- `nix-hash`
- `nix-instantiate`
- `nix-prefetch-url`
- `nix-prefetch-git`

- `nixos-option`

### Tools

- [nixops](https://github.com/NixOS/nixops) - deploying to nixOS machines in a network or the cloud.
- [nix-deploy](https://github.com/awakesecurity/nix-deploy), [Deploy software easily and securely using nix-deploy](https://awakesecurity.com/blog/deploy-software-easily-securely-using-nix-deploy/)
- [hocker](https://github.com/awakesecurity/hocker), [Hocker, I can't believe it's not docker!](http://ixmatus.net/articles/docker-without-docker.html), [Integration woes with docker containers and NixOS](http://ixmatus.net/articles/hocker-nixos-docker.html)
- [disnix](https://github.com/svanderburg/disnix) - distributed service deployment extension for the Nix package manager

- [kubenix](https://github.com/xtruder/kubenix) - Kubernetes resource builder written in nix (WIP)


- [lorri](https://github.com/target/lorri) - `nix-shell` replacement for project development
- [niv](https://github.com/nmattia/niv) - Painless dependencies for Nix projects
- [styx](https://github.com/jyp/styx) - a nix-based multi-repo Haskell project manager

### Services

- [cachix](https://cachix.org/) - Remote shared cache as a service.
- [nixbuild](https://docs.nixbuild.net/) - Remote building machine as a service

### Nix Expression Language

- [Short Language Overview](https://nixos.wiki/wiki/Nix_Expression_Language)
- [Typed Nix programming using Dhall](http://www.haskellforall.com/2017/01/typed-nix-programming-using-dhall.html) - Typing nix
- [dhall-nix](https://hackage.haskell.org/package/dhall-nix) - dhall to nix compiler

### Nixpkgs

- [fetchTarball vs fetchGit vs fetchFromGithub](https://discourse.nixos.org/t/difference-between-fetchtarball-fetchfromgithub-fetchgit/3279)
- [Import From Derivation](https://nixos.wiki/wiki/Import_From_Derivation)
- [Overlays and Overriding a package inside a scope](https://nixos.wiki/wiki/Overlays) - Overriding a package inside a scope, Python Packages Overlay
- [NixOS: The DOs and DON’Ts of nixpkgs overlays](https://blog.flyingcircus.io/2017/11/07/nixos-the-dos-and-donts-of-nixpkgs-overlays/)
- [packageSourceOverrides](https://github.com/NixOS/nixpkgs/blob/7d30b4d1b57fc6fb11b0b34aea9fd313d40447d4/pkgs/development/haskell-modules/lib.nix#L47) - Automatically call `callCabal2nix` or `callHackage`. [Here is an example](https://github.com/Gabriel439/Haskell-Turtle-Library/blob/master/default.nix#L18)
- [Contributing to Nixpkgs](https://rawkode.com/articles/contributing-nixpkgs/) - Adding an extension to gnome-3 (good read)
- [Updating your Nix Sources](https://garbas.si/2016/updating-your-nix-sources.html) - The repo is very interesting, I can't say the same about the blog.
- [Getting ghcide into nixpkgs](https://mpickering.github.io//ide/posts/2020-06-05-ghcide-and-nixpkgs.html) - Full of details (recommended)
- [haskellPackages.stm-containers fails to build](https://discourse.nixos.org/t/haskellpackages-stm-containers-fails-to-build/5416/4) - How to solve the issue with a lot of details. `haskell2nix` explained.

### NixOS

- [How to add <nixos-unstable> channel declaratively in configuration.nix](https://stackoverflow.com/questions/48831392/how-to-add-nixos-unstable-channel-declaratively-in-configuration-nix)
- [How to add <nixos-unstable> channel declaratively in configuration.nix: 2nd part](https://stackoverflow.com/questions/48838411/install-virtualbox-modules-from-nixos-unstable-in-configuration-nix/48842655#48842655)
- [Overriding some packages](https://stackoverflow.com/questions/36000514/how-to-override-2-two-packages-in-nixos-configuration-nix), [Overriding a haskell package](https://unix.stackexchange.com/questions/497798/how-can-i-override-a-broken-haskell-package-in-nix)
- (outdated)[Install NixOS on Amazon EC2](https://nixos.wiki/wiki/Install_NixOS_on_Amazon_EC2)
- [nixos-infect](https://github.com/elitak/nixos-infect) - install NixOS on Digital Ocean droplets, Vultr servers, or OVH Virtual Private Servers

NixOS in production

- [NixOS in production](http://www.haskellforall.com/2018/08/nixos-in-production.html) - short post summarizing what I wish I had known when I first started using NixOS in production
- [Deploy software easily and securely using nix-deploy](https://awakesecurity.com/blog/deploy-software-easily-securely-using-nix-deploy/)

### Projects using Nix

- [release-services](https://github.com/mozilla/release-services/tree/master/nix) - mozilla project with HEAVY use of nix.

### Youtube

- [Chris Martin - Deploying Haskell to the Cloud (part 1 & 2 / 4)](https://www.youtube.com/watch?v=DQ44q2aIP48&list=PLcAu_kKy-krz3t2teYyCM0Lt4015DF-Zp&index=22&t=0s)

### Tricks & tips

- The default script for each phase is defined in the file `pkgs/stdenv/generic/setup.sh`.

- See the sources of a package:

```bash
$ nix edit -f '<nixpkgs>' hello
```

- Get the derivation of a closure:

```bash
$ pretty-derivation < $(nix-store -qd $(which arandr))
```

- Print runtime dependencies of a closure:

```bash
$ nix-store -qR $(which svn)
```

- Get a haskell package version:

```bash
$ nix-instantiate '<nixpkgs>' --eval --strict --attr haskellPackages.hocker.version
```

- `patchShebangs`, `makeWrapper`, etc (search `grep -R 'callPackageWith =' .`): https://github.com/NixOS/nixpkgs/tree/master/pkgs/build-support/setup-hooks

- Nix Channel Status: https://status.nixos.org/

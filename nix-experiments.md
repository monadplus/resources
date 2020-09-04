Nix Experiments
===============

- Custom environment using `packageOverrides`:

```nix
# foo.nix
let config = {
  packageOverrides = pkgs: with pkgs; {
      myPackages = pkgs.buildEnv {
        name = "foo";
        paths = [
          nox
        ];
        pathsToLink = [ "/share" "/bin" ];
      };
    };
  };
  pkgs = import <nixpkgs> { inherit config; };

in pkgs
```

```bash
# Execute it likes these.
$ nix-shell foo.nix -A myPackages
```

Nixpkgs
=======

### Common Functions

- `callPackageWith`:

```nix
/* Call the package function in the file `fn' with the required
  arguments automatically.  The function is called with the
  arguments `args', but any missing arguments are obtained from
  `autoArgs'.  This function is intended to be partially
  parameterised, e.g.,

    callPackage = callPackageWith pkgs;
    pkgs = {
      libfoo = callPackage ./foo.nix { };
      libbar = callPackage ./bar.nix { };
    };
*/
callPackageWith = autoArgs: fn: args:
  let
    f = if lib.isFunction fn then fn else import fn;
    auto = builtins.intersectAttrs (lib.functionArgs f) autoArgs;
  in makeOverridable f (auto // args);
```

- `callPackage` file_to_import:path args:set.

- `buildEnv`: creates a tree of symlinks to the specified paths

- `newScope` (from pkgs/top-level/splice.nix): similar to `callPackageWith`

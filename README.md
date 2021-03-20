# buildroot
Build environment for the Flutter engine

This repository is used by the [flutter/engine](https://github.com/flutter/engine) repository.
For instructions on how to use it, see that repository's [CONTRIBUTING.md](https://github.com/flutter/engine/blob/master/CONTRIBUTING.md) file.

To update your checkout to use the latest buildroot, run `gclient sync`.

To submit patches to this buildroot repository, create a branch, push to that branch, then submit a PR on GitHub for that branch.

To point the engine to a new version of buildroot after your patch is merged, update the buildroot hash in the engine's [DEPS file](https://github.com/flutter/engine/blob/master/DEPS).


# gclient sample
```
solutions = [
    {
        "managed": False,
        "name": "src/flutter",
        "url": "https://github.com/LibertyGlobal/flutter-tvos-engine.git@1.26.0-17.6.pre",
        "custom_deps": {},
        "deps_file": "DEPS",
        "safesync_url": ""
    }
]
```
# NOTICE

This repository exists only to solve https://github.com/phadej/qc-instances/issues/9 If you are facing the same issue, please add the following to the `packages` section in your `stack.yaml` file. Please note, this will give you a patched version of **v0.3.12 of the quickcheck-instances package**

```
packages:
- location:
    git: git@github.com:vacationlabs/qc-instances.git
    commit: 29fa5cfd58371dcb3e6a5e672c755180fec95af6
```

# quickcheck-instances [![Build Status](https://travis-ci.org/aslatter/qc-instances.svg?branch=master)](https://travis-ci.org/aslatter/qc-instances)

This package provides instances for the classes in the QuickCheck Haskell library.

QuickCheck itself doesn't ship with instances for types outsde of the `base` package, however there are a lot more types which are commonly used within Haskell libraries and programs.

We aim to provide instances for the types which ship with the Haskell Platform, however we only add them as the maintainer needs them or as patches are received, so we may lag behind the platform itself.

Patches are always welcome!

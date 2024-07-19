# kondo-repro-unused

## To exhibit the issue

```sh
$ clj-kondo --version
clj-kondo v2024.05.24
```

```sh
$ clj-kondo --lint src/
linting took 25ms, errors: 0, warnings: 0
```

## Expected

```sh
$ clj-kondo --lint src/
src/kondo_repro_unused/core.clj:3:5: warning: namespace kondo-repro-unused.core
is required but never used
linting took 15ms, errors: 0, warnings: 1
```

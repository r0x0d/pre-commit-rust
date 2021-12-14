[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/r0x0d/pre-commit-rust/master.svg)](https://results.pre-commit.ci/latest/github/r0x0d/pre-commit-rust/master)

# Rust hooks for pre-commit

[Rust](https://www.rust-lang.org) tools package for [pre-commit](https://pre-commit.com).

## Using rust tools with pre-commit

```yaml
-   repo: https://github.com/r0x0d/pre-commit-rust
    rev: master
    hooks:
    -   id: fmt
    -   id: check
    -   id: clippy
```

## Passing arguments to rustfmt

```yaml
-   repo: https://github.com/r0x0d/pre-commit-rust
    rev: master
    hooks:
    -   id: fmt
        args: ['--verbose', '--edition', '2018', '--']
```

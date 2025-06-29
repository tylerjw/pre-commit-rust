# Rust hooks for pre-commit

[Rust](https://www.rust-lang.org) tools package for [pre-commit](https://pre-commit.com).

## Using rust tools with pre-commit

```yaml
repos:
  - repo: https://github.com/tylerjw/pre-commit-rust.git
    rev: v1.8
    hooks:
      - id: fmt
      - id: check
      - id: clippy
      - id: machete
      - id: sort
      - id: sort-derives
```

## Passing arguments to rustfmt

```yaml
repos:
  - repo: https://github.com/tylerjw/pre-commit-rust.git
    rev: v1.8
    hooks:
      - id: fmt
        args: ['--verbose', '--edition', '2018', '--']
```

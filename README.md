# Stylus Sprint - ArbOs Foundry Mono

The repository is a single point for developing and building arbos-foundry. 

## Getting started

### Prerequisites

* Rust 1.84
* Docker
* Stylus develop prerequisites - https://docs.arbitrum.io/stylus/quickstart

### Clone 

```bash
git clone --recurse https://github.com/iosiro/arbos-foundry-mono.git && arbos-foundry-mono
```

### Make nitro

We need to make call `make` in the nitro directory to precompile the static libraries for `brotli`.

```bash
cd nitro && make
```

## Run integration tests

Integrations tests are developed in a separate repository to minimize the `diff` size of revm. 

```bash
cd revm-tests && cargo test
```
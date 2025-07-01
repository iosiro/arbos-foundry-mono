# Prerequisites (MacOS)

* LLVM (brew install llvm)
* LLD (brew install lld)
* Node 18
* Docker
* Stylus develop prerequisites - https://docs.arbitrum.io/stylus/quickstart


# Building

```
git clone --recurse 
```

```
cd nitro &&  make wasm-ci-build
```

```
cd arbos-foundry && cargo build --release && export PATH=$PATH:$(pwd)/target/release
```


# Using

Use `arbos-forge` as normal from within a Foundry project.

```
arbos-forge test 
```
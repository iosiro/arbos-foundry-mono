# Prerequisites (MacOS)

* LLVM (brew install llvm)
* LLD (brew install lld)
* Node 18


# Building

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
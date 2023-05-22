To deploy Rust contract on the Golden Gate network you can follow video tutorials <https://youtu.be/xl-QliBpH9k> and <https://youtu.be/Zp1JtBYxXJg> or follow the steps.

#### Update Your Development Environment ####

1. Update Rust using `rustup compnent add rust-src`
2. Verify that you have the WebAssembly target installed using `rustup target add wasm32-unknown-unknown --toolchain nightly`
**Install cargo-contract** 
cargo-contract is a command-line tool which you will use to build, deploy, and interact with your ink! contracts. You can install it using `cargo install --force --locked cargo-contract --version 2.0.0-rc`
**Compile your contract into [WASM][wasm]**
To build contract using cargo navigate to the folder with contract and run `cargo contract build`
**Deploy your contract on the Golden Gate**
1. Navigate to explorer of the Golden Gate network you want to deploy your contract on (<https://testnet.brooklyn.ggxchain.io/> for the Brooklyn testnet)
2. Go to Developer-->Contracts page
3. Press Upload & deploy code
4. Choose deployment account (you will need [PolkadotJS][polkadotjs] or other substrate account manager to use your account)
[wasm]./wasm.md
[polkadots]./polkadotjs.md
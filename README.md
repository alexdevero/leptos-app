# Leptos Web App

This application is built using the Leptos framework for Rust. This README will guide you through setting up your environment and running the app locally.

## Prerequisites

- Rust: You should have Rust installed on your machine. You can download it [here](https://www.rust-lang.org/tools/install).

## Getting Started

This tutorial uses Trunk for client-side rendering.

1. **Install Trunk**: If not already installed, Trunk can be installed by running the command:

```shell
cargo install trunk
```

2. **Switch to Nightly Rust**: This tutorial recommends using Nightly Rust. To use Nightly Rust with WebAssembly, run the following commands:

```shell
rustup toolchain install nightly
rustup default nightly
```

3. **Add wasm32 target**: Add wasm32-unknown-unknown target so that Rust can compile your code to WebAssembly to run in the browser.

```shell
rustup target add wasm32-unknown-unknown
```

4. **Run the application**: Now run the following command from the root of the leptos-app directory. Trunk should automatically compile the app and open it in your default browser. If you make edits to main.rs, Trunk will recompile your source code and live-reload the page.

```shell
trunk serve --open
```

With that, you should have the app running on your local machine.

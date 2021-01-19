# My Dapp

This project is for the blockchain application My Dapp. It contains code for the Smart Contract, web-based dapp and NodeJS server. 

# Pre-requisites

In order to develop and build "My Dapp," the following pre-requisites must be installed:

* [Visual Studio Code](https://code.visualstudio.com/download) (or any IDE for editing Javascript)
* [NodeJS](https://nodejs.org/en/download/)
* [Yarn](https://classic.yarnpkg.com/en/docs/install) (DappStarter uses [Yarn Workspaces](https://classic.yarnpkg.com/en/docs/workspaces))
* [Solana CLI Tools](https://docs.solana.com/cli/install-solana-cli-tools)
* Rust (see "Dependency Guides" at the end for help installing)

### Dependency Checklist 
```bash
$ node --version
$ npm --version
$ rustup --version
$ rustc --version
$ cargo --version
$ solana --version
```

# Installation

Using a terminal (or command prompt), change to the folder containing the project files and type: `yarn` This will fetch all required dependencies. The process will take 1-3 minutes and while it is in progress you can move on to the next step.

# Build, Deploy and Test
Using a terminal (or command prompt), change to the folder containing the project files and type: `yarn start` This will run all the dev scripts in each project package.json.

To view your dapp, open your browser to http://localhost:5000

We ♥️ developers and want you to have an awesome experience. You should be experiencing Dappiness at this point. If not, let us know and we will help. Visit [https://support.trycrypto.com](https://support.trycrypto.com) or hit us up on Twitter @decentology.


## Smart Contract

`yarn migrate` to compile contracts/*.sol files, deploy them to the blockchain. 

## Dapp

Run the dapp in a separate terminal. You *must* have run `npm run deploy` for the dapp to see most recent smart contract changes.

`yarn dapp` runs the dapp on http://localhost:5001 using webpack dev server

## Server

Run the server in a separate terminal. You *must* have run `npm run deploy` for the dapp to see most recent smart contract changes.

`yarn server` runs NodeJS server app on port 5002 with NestJS

## Production Builds

DappStarter currently does not provide blockchain migration scripts to be used in production. However, here are the scripts for generating production builds:

`yarn build:prod` generates dapp bundle for production.

## Dependency Guides

This section contains installation guides for common dev environments. 

### Rust

(Source: Solana)
We suggest that you install Rust using the 'rustup' tool. Rustup will install
the latest version of Rust, Cargo, and the other binaries.

Follow the instructions at [Installing Rust](https://www.rust-lang.org/tools/install).

For Mac users, Homebrew is also an option.  The Mac Homebrew command is `brew install rustup` and then
`rustup-init`. See [Mac Setup](https://sourabhbajaj.com/mac-setup/Rust/) &
[Installing Rust](https://www.rust-lang.org/tools/install) for more details.

After installation, you should have `rustc`, `cargo`, & `rustup`. You should
also have `~/.cargo/bin` in your PATH environment variable.


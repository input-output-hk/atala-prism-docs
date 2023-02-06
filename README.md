# Atala Prism V2 documentation website

This website is built using [Docusaurus 2](https://docusaurus.io/).

# Structure

The `documentation` folder is split into the following parts:
* `docs`
* `tutorials`
* `sdk`
* `api`

## `docs`: general documentation

`documentation/docs` is a general documentation directory for:
* Getting started guides
* SSI and Atala concepts
* Atala PRISM architecture and components description

## `tutorials`: general Atala PRISM tutorials

`documentation/tutorials`  directory assigned to contain all tutorials about essential topics and protocols Atala PRISM V2 is supported, for example:
* Credential issuance
* Verification
* DIDs
* etc.

## `sdk`: SDKs documentation

`documentation/sdk` is a special directory for SDK documentation, user guides, and examples. There are two subfolders:
* `enterprise-sdk`: for what we call now "Enterprise SDK"
* `wallet-sdk`: for what we call now "Wallet SDK"

## `api`: autogenerated docs from OpenAPI specs

`documentation/api` directory contains auto-generated documentation for RestAPI endpoints provided by Atala PRISM V2 executables, it's auto-generated and should not be added manually.

## Installation

Here are the simple installation instructions for MacOS to start from the very scratch.

```shell
# Install brew, git, node and yarn
# if you 
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install git
brew install node
brew install yarn

# Create new projects directory
cd ~ && mkdir projects && cd projects
git clone https://github.com/input-output-hk/atala-prism-docs.git

# Deploy local version of the website
cd atala-prism-docs
yarn install
yarn docusaurus gen-api-docs all
yarn start
```

## Local Development

```
$ yarn start
```

This command starts a local development server and opens up a browser window. Most changes are reflected live without having to restart the server.

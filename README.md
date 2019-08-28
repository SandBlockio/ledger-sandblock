# Ledger-Sandblock

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

This repository contains two Ledger Nano S apps for Tendermint/Sandblock:

-   Ledger Nano S Sandblock BOLOS app
-   Ledger Nano S Tendermint validator BOLOS app
-   C++ unit tests

Source code for apps is linked as submodules to allow for Ledger's build infrastructure.

For development purposes, this repo is recommended as it includes unit tests, tools, etc.

---

## Installing

### Sandblock app

The Sandblock app is not yet available on Ledger Live.
The documentation will be updated as soon as the app is made available.

### Tendermint Validator app

The validator app is available in [Ledger Live](https://www.ledger.com/pages/ledger-live).

**The app has been released in TEST mode for now! WARNING: It is possible to exit without unplugging**

![](docs/img/cosmos_app1.png)

-   Enable developer mode (last option):

![](docs/img/cosmos_app2.png)

To install, please follow the build instructions in the following section.

-   Now go back to manager and search for Tendermint:

![](docs/img/tendermint_app.png)

---

## Building

The following document describes how to build the apps: [Build instructions](docs/BUILD.md)

---

## Specifications

### Sandblock App

-   [APDU Protocol](https://github.com/SandBlockio/ledger-sandblock-app/tree/master/docs/APDUSPEC.md)
-   [Transaction format](https://github.com/SandBlockio/ledger-sandblock-app/tree/master/docs/TXSPEC.md)
-   [User interface](https://github.com/SandBlockio/ledger-sandblock-app/tree/master/docs/UISPEC.md)

### Validator App

The target of this app are validators. The app signs votes/proposals via the Tendermint/Cosmos KMS (Key management system).

### Specifications

-   [APDU Protocol](https://github.com/tendermint/ledger-validator-app/blob/master/docs/APDUSPEC.md)
-   [Transaction format](https://github.com/tendermint/ledger-validator-app/blob/master/docs/TXSPEC.md)
-   [User interface](https://github.com/tendermint/ledger-validator-app/blob/master/docs/UISPEC.md)

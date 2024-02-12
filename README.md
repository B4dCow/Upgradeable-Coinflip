## Proxy Comparison (Transparent Proxy Model & UUPS Proxy Model )

In the Transparent Proxy Model, the proxy contract delegates all calls to an implementation contract, and the implementation contract's address is set at the time of deployment. This means that the implementation contract cannot be changed without deploying a new proxy contract. 

On the other hand, the UUPS Proxy Model allows for the upgrade of the implementation contract without changing the proxy contract's address. This is achieved by using a two-step delegate call, which enables the proxy contract to be upgraded while preserving its address and state. 

Both models aim to provide upgradability for smart contracts, but they differ in how they handle the relationship between the proxy and implementation contracts, with the UUPS Proxy Model offering more flexibility in upgrading the implementation contract without changing the proxy contract's address.


## Foundry

**Foundry is a blazing fast, portable and modular toolkit for Ethereum application development written in Rust.**

Foundry consists of:

-   **Forge**: Ethereum testing framework (like Truffle, Hardhat and DappTools).
-   **Cast**: Swiss army knife for interacting with EVM smart contracts, sending transactions and getting chain data.
-   **Anvil**: Local Ethereum node, akin to Ganache, Hardhat Network.
-   **Chisel**: Fast, utilitarian, and verbose solidity REPL.

## Documentation

https://book.getfoundry.sh/

## Usage

### Build

```shell
$ forge build
```

### Test

```shell
$ forge test
```

### Format

```shell
$ forge fmt
```

### Gas Snapshots

```shell
$ forge snapshot
```

### Anvil

```shell
$ anvil
```

### Deploy

```shell
$ forge script script/Counter.s.sol:CounterScript --rpc-url <your_rpc_url> --private-key <your_private_key>
```

### Cast

```shell
$ cast <subcommand>
```

### Help

```shell
$ forge --help
$ anvil --help
$ cast --help
```

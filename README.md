# areoncli

#### AreonCLI is an all-in-one command line tool. It enables users to see their transactions and run some of the functions easily. 

####  The CLI, can receive commands to be able to run various processes and communicate with the network. Thanks to the features of AreonCLI performing different tasks and managing the network efficiently is now easy.

## https://hub.docker.com/repository/docker/areonnetwork/areoncli

## Example commands

Help commands (--help)

Get important information for the server with cli.

Usage:
  areoncli [flags]
  areoncli [command]

Available Commands:
  balance     Get balance
  block       Get block details
  calculate   Calculate currency
  completion  Generate the autocompletion script for the specified shell
  create      Create a new wallet
  hash        Get transaction details by hash
  help        Help about any command
  validator   Validator process

Flags:
      --chain string   Blockchain network type (mainnet or testnet) (default "mainnet")
  -h, --help           help for areoncli
  -v, --version        version for areoncli

Use "areoncli [command] --help" for more information about a command.

```
./areoncli --help
```
-------------

Calculate Price Run:

The command calculates the equivalent amount of AREA/USDT for the entered amount.

```
./areoncli calculate [amount]
```
-------------

Terminal Run:

- Mainnet and Testnet terminal.

- According to the chain tip, "mainnet" or "testnet" should be used.

- You can exit using the "Q" key or by typing "exit".

```
./areoncli --chain [chaintype]
```
-------------
Create Wallet Run:

- The command used to create a wallet.

- Returns Public Key, Private Key, and EVM Address.

```
./areoncli create wallet
```
-------------

Balance Result Run:

- Command that gives "Balance" value according to Account address.

- Displays the balance amounts in all chain wallets.

```
./arencli balance [address]
```
-------------

Transaction Hash:

- Provides transaction details based on the hash information.

- It depends on the chain tip. If "testnet" is desired, then "--chain testnet" should be used.

```
./areoncli hash [txhash]
```
-------------

Block Run:

- It provides information about the block based on the block number.

- It depends on the chain tip. If "testnet" is desired, then "--chain testnet" should be used.

```
./areoncli block [blocknumber]
```
-------------

Connect Run:

The command creates and checks the validator's block validation status and the node's connection to the network.

```
./areoncli validator connect [identity]
```
-------------

Stats Run:

The command shows the details of the validator's quantities and sync status.

```
./areoncli validator stats [identity]
```
-------------

Delegation Run:

The command lists validator delegations by address and amount.

```
./areoncli validator delegations [identity]
```
-------------

Unjail Run:

The command is used to reactivate the validator if it has been jailed.

```
./areoncli validator unjail [identity]
```
-------------

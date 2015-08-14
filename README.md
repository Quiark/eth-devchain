# eth-devchain: quick & dirty private testnet


These files let you run geth on your own private chain for contract development.
A private chain lets you mine your blocks quickly and easily and you can have all the
ether you'll ever need for development.

## Usage

Edit `private_genesis.json` as you need, perhaps you'd like to increase the account's funds.
I recommend keeping the difficulty pretty low too, it makes the DAG faster to compute.

When done, run the command from `private_geth.ps1`. Note that:

* the command there enables ALL management APIs to the RPC which would be a totally unsafe thing to do on the livenet
* you may want to change networkid to a random number
* you may need to change the path to solidity compiler solc (can be downloaded with the cpp-ethereum or eth++ package)


## Private key
I also provide the private key for the account pre-funded in genesis. The password is `abcd`.

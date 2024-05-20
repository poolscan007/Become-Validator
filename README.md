# Become-Validator


Git clone https://github.com/MEDIABLOCKAI/validator-setup

Create an Account

chmod +x openethereum
./openethereum account new --config ./node.toml
Returned address like that 0x00aa39d30f0d20ff03a22ccfc30b7efbfca597c2

Copy result address to mode.toml Ex:

...
[account]
unlock = ["0x00aa39d30f0d20ff03a22ccfc30b7efbfca597c2"]
password = ["password"]

[mining]
force_sealing = true
engine_signer = "0x00aa39d30f0d20ff03a22ccfc30b7efbfca597c2"
reseal_on_txs = "none"
...
Run the authority nodes
./openethereum --config ./node.toml

Stake

Stake

To stake MBC coin, all you should do is sending your MBC coin to the MBC Consensus contract address over the MBC network from the validator address. The MBC Consensus contract address: 0x7eFb6A569C57e2c40DCa3533b47B3EC9ce69529f The easiest way to do so, is to import your private key or key-store file to your favourite wallet (for example Metamask), switch network to MBC and send the MBC coin to the Consensus contract address.

You can find your key-store (containing your private key) and the password for the created account in: /node/keys/MBC/UTC--xxxx /node.pwd

Wait for 1 cycle (approximately 48 hours).

Wait until the next cycle gets started.

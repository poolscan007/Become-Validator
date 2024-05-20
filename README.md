# Become-Validator


Git clone 

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

To stake PSC coin, all you should do is sending your 100000 PSC coin to the PSC Consensus contract address over the PSC network from the validator address. The PSC Consensus contract address: 0xd3c951B3A691d3deAA3D95221Fd6332683C2eBA9 The easiest way to do so, is to import your private key or key-store file to your favourite wallet (for example Metamask), switch network to PSC and send the PSC coin to the Consensus contract address.

You can find your key-store (containing your private key) and the password for the created account in: /node/keys/PSC/UTC--xxxx /node.pwd

Wait for 1 cycle (approximately 48 hours).

Wait until the next cycle gets started.

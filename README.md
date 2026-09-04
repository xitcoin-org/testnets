# Xitcoin Testnets

Canonical genesis and public configuration files for Xitcoin test networks.

## Active public testnet

| Parameter | Value |
| --- | --- |
| Network | Xitcoin Public Testnet |
| Cosmos chain ID | `xitcoin-testnet-v2-1` |
| EVM chain ID | `101089` (`0x18ae1`) |
| Native symbol | `XTC` |
| Base denomination | `axtc` |
| Decimals | `18` |
| Genesis supply | `477,000,000 XTC` |
| Genesis SHA-256 | `5db34acf6496b2c76a6f516e0eb605caef6762552584ddbed7c8703239f33d72` |
| Initial validators | `4` |
| Validator capacity | `258` |
| Minimum self-delegation | `5,000,000 XTC` |
| Public faucet | `10 XTC` per successful request |
| Bridge route | Disabled; not configured |

The active network files are stored in [`xitcoin-testnet-v2-1`](./xitcoin-testnet-v2-1).

Verify the byte-identical genesis file with:

```bash
cd xitcoin-testnet-v2-1
sha256sum -c genesis.sha256
```

## Retired networks

[`xitcoin-testnet-1`](./xitcoin-testnet-1) is retained only for historical verification. It is not active and must not be used for new deployments or transactions.

Private keys, mnemonics, keyrings, passwords, runtime state and validator backups must never be committed to this repository.

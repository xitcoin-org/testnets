# Xitcoin Testnets

Canonical genesis and public configuration files for Xitcoin test networks.

## Active public testnet

| Parameter | Value |
| --- | --- |
| Network | Xitcoin Testnet |
| Cosmos chain ID | `xitcoin-testnet-1` |
| EVM chain ID | `101089` (`0x18ae1`) |
| Native symbol | `XTC` |
| Base denomination | `axtc` |
| Decimals | `18` |
| Genesis supply | `457,000,000 XTC` |
| Genesis SHA-256 | `55c8756a212b9e92c0e8427ea61caff7fa9dca40e801e4b848f59d1aa5f6dae6` |
| Initial validators | `4` |
| Validator capacity | `258` |
| Minimum self-delegation | `5,000,000 XTC` |
| Public faucet | `10 XTC` per successful request |
| Bridge route | Disabled; not configured |

The active network files are stored in [`xitcoin-testnet-1`](./xitcoin-testnet-1).

The published genesis is byte-identical to the genesis deployed on the canonical
sentry and four validators. Verify it with:

```bash
cd xitcoin-testnet-1
sha256sum -c genesis.sha256
```

The faucet allocation is finite and does not mint XTC automatically. The
canonical metadata in [`chain.json`](./xitcoin-testnet-1/chain.json) records
the public endpoints, allocation categories and validator policy.

Private keys, mnemonics, keyrings, passwords, runtime state and validator
backups must never be committed to this repository.

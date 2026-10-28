<!-- gully-header:start -->
<p align="center">
  <a href="https://gullychain.xyz">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset=".github/assets/gullychain-wordmark-for-dark-bg.png">
      <img alt="Gully Chain" src=".github/assets/gullychain-wordmark-for-light-bg.png" width="360">
    </picture>
  </a>
</p>

<p align="center"><b>The social chain where your profile is your wallet. Arbitrum Orbit L3, testnet chain 485590.</b></p>

<p align="center">ERC-4337 bundler for Gully Chain profile wallets.</p>

<p align="center">
  <a href="https://gullychain.xyz"><img src="https://img.shields.io/badge/gullychain.xyz-01D9FA?style=for-the-badge&labelColor=000000&logo=googlechrome&logoColor=000000" alt="Website"></a>
  <a href="https://docs.gullychain.xyz"><img src="https://img.shields.io/badge/Docs-0A0F1A?style=for-the-badge&labelColor=000000&logo=readthedocs&logoColor=01D9FA" alt="Docs"></a>
  <a href="https://t.me/GullyChain"><img src="https://img.shields.io/badge/Telegram-0A0F1A?style=for-the-badge&labelColor=000000&logo=telegram&logoColor=26A5E4" alt="Telegram"></a>
  <a href="https://discord.com/invite/tY2ErsNNBp"><img src="https://img.shields.io/badge/Discord-0A0F1A?style=for-the-badge&labelColor=000000&logo=discord&logoColor=5865F2" alt="Discord"></a>
  <a href="https://x.com/Gully_Labs"><img src="https://img.shields.io/badge/@Gully__Labs-0A0F1A?style=for-the-badge&labelColor=000000&logo=x&logoColor=white" alt="X"></a>
</p>

<p align="center"><sub>A Gully Chain fork of <a href="https://github.com/pimlicolabs/alto">pimlicolabs/alto</a>, maintained by <a href="https://gullylabs.xyz">Gully Labs</a>. It is used under its GPL-3.0 licence; the upstream LICENSE, copyright and attribution notices are kept unchanged. The upstream README follows below as published. Not affiliated with or endorsed by pimlicolabs.</sub></p>

---
<!-- gully-header:end -->

<p align="center"><a href="https://docs.pimlico/reference/bundler"><img width="1000" title="Alto" src='https://i.imgur.com/qgVAdjN.png' /></a></p>

# ⛰️ Alto ⛰️

![Node Version](https://img.shields.io/badge/node-20.x-green)

Alto is a Typescript implementation of the [ERC-4337 bundler specification](https://eips.ethereum.org/EIPS/eip-4337) developed by [Pimlico](https://pimlico.io), focused on transaction inclusion reliability.

## Getting started

For a full explanation of Alto, please visit our [docs page](https://docs.pimlico.io/infra/bundler)

#### Run an instance of Alto with the following commands:
```bash
pnpm install
pnpm build:all
./alto --entrypoints "0x5ff1...2789,0x0000...a032" --executor-private-keys "..." --utility-private-key "..." --min-balance "0" --rpc-url "http://localhost:8545" --network-name "local"
```
To find a list of all options, run:
```bash
./alto help
```

A helper script for running Alto locally with an Anvil node can be found at [scripts/run-local-instance.sh](scripts/README.md).

A comprehensive guide for self-hosting Alto can be found [here](https://docs.pimlico.io/infra/bundler/self-host).

#### Run the test suite with the following commands:
```bash
pnpm build
pnpm test # note: foundry must be installed on the machine for this to work
```

## Prerequisites

- :gear: [NodeJS](https://nodejs.org/) (LTS)
- :toolbox: [Pnpm](https://pnpm.io/)

## How to run E2E tests

- pnpm run test

## How to test bundler specs

- Run Geth node or any other node that support debug_traceCall
- Clone [bundler-spec-tests](https://github.com/eth-infinitism/bundler-spec-tests) repo.
- build & run bundler with `--environment development --bundleMode manual --safeMode true`


## License

Distributed under the GPL-3.0 License. See [LICENSE](./LICENSE) for more information.

## Contact

Feel free to ask any questions in our [Telegram group](https://t.me/pimlicoHQ)

## Acknowledgements

- [Eth-Infinitism bundler](https://github.com/eth-infinitism/bundler)
- [Lodestar](https://github.com/ChainSafe/lodestar)


<!-- gully-footer:start -->
---

<p align="center">
  <a href="https://gullylabs.xyz">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset=".github/assets/powered-by-gully-labs-dark-2x.png">
      <img alt="Powered by Gully Labs" src=".github/assets/powered-by-gully-labs-light-2x.png" width="254" height="64">
    </picture>
  </a>
</p>
<!-- gully-footer:end -->

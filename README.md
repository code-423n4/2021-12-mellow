# ✨ So you want to sponsor a contest

This `README.md` contains a set of checklists for our contest collaboration.

Your contest will use two repos:

- **a _contest_ repo** (this one), which is used for scoping your contest and for providing information to contestants (wardens)
- **a _findings_ repo**, where issues are submitted.

Ultimately, when we launch the contest, this contest repo will be made public and will contain the smart contracts to be reviewed and all the information needed for contest participants. The findings repo will be made public after the contest is over and your team has mitigated the identified issues.

Some of the checklists in this doc are for **C4 (🐺)** and some of them are for **you as the contest sponsor (⭐️)**.

---

# Contest setup

## 🐺 C4: Set up repos

- [x] Create a new private repo named `YYYY-MM-sponsorname` using this repo as a template.
- [ ] Get GitHub handles from sponsor.
- [ ] Add sponsor to this private repo with 'maintain' level access.
- [ ] Send the sponsor contact the url for this repo to follow the instructions below and add contracts here.
- [ ] Delete this checklist and wait for sponsor to complete their checklist.

## ⭐️ Sponsor: Provide contest details

Under "SPONSORS ADD INFO HERE" heading below, include the following:

- [ ] Name of each contract and:
  - [ ] lines of code in each
  - [ ] external contracts called in each
  - [ ] libraries used in each
- [ ] Describe any novel or unique curve logic or mathematical models implemented in the contracts
- [ ] Does the token conform to the ERC-20 standard? In what specific ways does it differ?
- [ ] Describe anything else that adds any special logic that makes your approach unique
- [ ] Identify any areas of specific concern in reviewing the code
- [ ] Add all of the code to this repo that you want reviewed
- [ ] Create a PR to this repo with the above changes.

---

# ⭐️ Sponsor: Provide marketing details

- [ ] Your logo (URL or add file to this repo - SVG or other vector format preferred)
- [ ] Your primary Twitter handle
- [ ] Any other Twitter handles we can/should tag in (e.g. organizers' personal accounts, etc.)
- [ ] Your Discord URI
- [ ] Your website
- [ ] Optional: Do you have any quirks, recurring themes, iconic tweets, community "secret handshake" stuff we could work in? How do your people recognize each other, for example?
- [ ] Optional: your logo in Discord emoji format

---

# Contest prep

## 🐺 C4: Contest prep

- [x] Rename this repo to reflect contest date (if applicable)
- [x] Rename contest H1 below
- [x] Add link to report form in contest details below
- [x] Update pot sizes
- [x] Fill in start and end times in contest bullets below.
- [ ] Move any relevant information in "contest scope information" above to the bottom of this readme.
- [ ] Add matching info to the [code423n4.com public contest data here](https://github.com/code-423n4/code423n4.com/blob/main/_data/contests/contests.csv))
- [ ] Delete this checklist.

## ⭐️ Sponsor: Contest prep

- [ ] Make sure your code is thoroughly commented using the [NatSpec format](https://docs.soliditylang.org/en/v0.5.10/natspec-format.html#natspec-format).
- [ ] Modify the bottom of this `README.md` file to describe how your code is supposed to work with links to any relevent documentation and any other criteria/details that the C4 Wardens should keep in mind when reviewing. ([Here's a well-constructed example.](https://github.com/code-423n4/2021-06-gro/blob/main/README.md))
- [ ] Please have final versions of contracts and documentation added/updated in this repo **no less than 8 hours prior to contest start time.**
- [ ] Ensure that you have access to the _findings_ repo where issues will be submitted.
- [ ] Promote the contest on Twitter (optional: tag in relevant protocols, etc.)
- [ ] Share it with your own communities (blog, Discord, Telegram, email newsletters, etc.)
- [ ] Optional: pre-record a high-level overview of your protocol (not just specific smart contract functions). This saves wardens a lot of time wading through documentation.
- [ ] Designate someone (or a team of people) to monitor DMs & questions in the C4 Discord (**#questions** channel) daily (Note: please _don't_ discuss issues submitted by wardens in an open channel, as this could give hints to other wardens.)
- [ ] Delete this checklist and all text above the line below when you're ready.

---

# Mellow Finance contest details

- $47,500 USDC main award pot
- $2,500 gas optimization award pot
- Join [C4 Discord](https://discord.gg/code4rena) to register
- Submit findings [using the C4 form](https://coderena.com/contests/2021-12-mellow-finance-contest/submit)
- [Read our guidelines for more details](https://docs.code4rena.com/roles/wardens)
- Starts December 2, 2021 00:00 UTC
- Ends December 8, 2021 23:59 UTC

This repo will be made public before the start of the contest. (C4 delete this line when made public)

# Welcome to Mellow Protocol 👾

![](https://github.com/code-423n4/2021-12-mellow/blob/main/bg.png)

Hello legends! 💪

🧐 We look forward to you dissecting our code and helping us improve the security! Feel free to ask any small or big questions, and ask for guidance or clarifications.

💬 Please pay attention to the docs and shoot any questions you have on Discord - we’ll be online to respond.

TBA - LOGO, etc

# Useful links 🧐

[Protocol documentation](https://docs.mellow.finance/) – the most complete information about the contracts

[Contract API](https://docs.mellow.finance/mellow-permissionless-vaults/api) - gitbook docs generated from contracts

[Vaults design article](https://mellowprotocol.medium.com/mellow-protocol-vaults-design-ed09bed7b869) – protocol design overview (A Medium article)

[Twitter](https://twitter.com/Mellowprotocol) | [Discord](https://discord.gg/w6sJDJrV65) | [Website](https://mellow.finance/)

# Contest Scope ✅

The following contracts are in scope:
|File|Comments|All lines of code (excluding Blank Lines and Comments)|Statements|Branches|Functions|Lines (excluding global variable declarations, function signatures , run over lines and event definitions)
|-|-|-|-|-|-|-|
||||||||
||||||||
||||||||
||||||||
||||||||
||||||||
||||||||
||||||||

## Contact us 📲

Feel free to ping us:

| Name | Discord       |
| ---- | ------------- |
| Alex | @AlexK#7957   |
| Mike | @mihanix#1481 |
| Nick | @0xn1ck#9123  |

We're happy to answer any questions and discuss every suggestion.

# Protocol overview 🔮

**We're buliding permissionless vaults ecosystem for trustless automatic DeFi strategies.
The protocol is designed for implementing multi-token cross-protocol liquidity rebalancing.**

The Vault contracts hold the tokens and rebalance them both inside other protocols and between them. Strategy contracts interact with Vault contracts definig the rebalancing parameters.

**Liquidity provider**
Users pick a strategy that fits their needs and allocate their assets into a vault to earn yield. When the assets are deposited, users get composable LP tokens (ERC-20).

**Strategies**
Strategies are smart-contracts that implement the models to provide effective liquidity allocation. Different market events can trigger the strategies to initiate rebalance.

**Vaults**
Vaults allocate multiple ERC-20 tokens into other DeFi protocols and rebalance the liquidity in accordance with Strategies inside and between the protocols.

A typical vault and strategy setup would be made by using Mellow Permissioless Vaults _deployVault_ function. As a result, the following set of smart contracts (called Vault System) would be established **for every strategy and token pair**:
![](https://miro.medium.com/max/1400/1*GeSO8eJ8WZUEjgko8V3LkQ.gif)

## Protocol architecture

![](https://miro.medium.com/max/2000/1*L4INk2ZLKCylmw1Yt28JTw.png)
There are two types of contracts on the diagram:

1.  **Protocol contracts** (pink color) — these are the protocol contracts that are deployed in one instance;
2.  **Vault contracts** (purple color) — these are the contracts deployed by users (vault owners/strategists) by using **protocol contracts.** Essentially everyone can create a set of Vault contracts.

We can logically separate contracts into Vault Groups. Each Vault Group is a set of contracts that allows managing and creating a vault of a specific Vault Kind. Vault Governance is a contract that can:

1.  Deploy a new vault via a VaultGovernance#deployVault method
2.  Manage governance params for specific vaults

Upon Vault creation, the Vault Registry contract mints a new ERC-721 token that represents that Vault.

## 📟 Contracts overview 📟

**AaveVault**

Vault that interfaces Aave protocol in the integration layer.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#aavevault).

**AaveVaultFactory**

Helper contract for `AaveVaultGovernance` that can create new Aave Vaults.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#aavevaultfactory).

**AaveVaultGovernance**

Governance that manages all Aave Vaults params and can deploy a new Aave Vault.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#aavevaultgovernance).

**YearnVault**

Vault that interfaces Yearn protocol in the integration layer.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#yearnvault).

**YearnVaultFactory**

Helper contract for `YearnVaultGovernance` that can create new Yearn Vaults.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#yearnvaultfactory).

**YearnVaultGovernance**

Governance that manages all Yearn Vaults params and can deploy a new Yearn Vault.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#yearnvaultgovernance).

**UniV3Vault**

Vault that interfaces UniV3 protocol in the integration layer.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#univ3vault).

**UniV3VaultFactory**

Helper contract for `UniV3VaultGovernance` that can create new UniV3 Vaults.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#univ3vaultfactory).

**UniV3VaultGovernance**

Governance that manages all UniV3 Vaults params and can deploy a new UniV3 Vault.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#univ3vaultgovernance).

**ERC20Vault**

Vault that stores ERC20 tokens.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#erc20vault).

**ERC20VaultFactory**

Helper contract for `ERC20VaultGovernance` that can create new ERC20 Vaults.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#erc20vaultfactory).

**ERC20VaultGovernance**

Governance that manages all ERC20 Vaults params and can deploy a new ERC20 Vault.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#erc20vaultgovernance).

**GatewayVault**

Vault that combines several integration layer Vaults into one Vault.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#gatewayvault).

**GatewayVaultFactory**

Helper contract for `GatewayVaultGovernance` that can create new Gateway Vaults.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#gatewayvaultfactory).

**GatewayVaultGovernance**

Governance that manages all Gateway Vaults params and can deploy a new Gateway Vault.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#gatewayvaultgovernance).

**LpIssuer**

Contract that mints and burns LP tokens in exchange for ERC20 liquidity.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#lpissuer).

**LpIssuerFactory**

Helper contract for `LpIssuerGovernance` that can create new Lp Issuers.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#lpissuerfactory).

**LpIssuerGovernance**

Governance that manages all LpIssuers params and can deploy a new LpIssuer.
[See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#lpissuergovernance).

**Vault**

Abstract contract that has logic common for every Vault. [See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#vault).

**VaultGovernance**

Internal contract for managing different params. [See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#vaultgovernance).

**ProtocolGovernance**

Governance that manages all params common for Mellow Permissionless Vaults protocol. [See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#protocolgovernance).

**DefaultAccessControl**

This is a default access control with 2 roles - ADMIN and ADMIN_DELEGATE. [See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#defaultaccesscontrol).

**CommonLibrary**

Common shared utilities

**ChiefTrader**

Main contract that allows trading of ERC20 tokens on different Dexes. [See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#chieftrader).

**UniV3Trader**

Contract that can execute ERC20 swaps on Uniswap V3. [See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#univ3trader).

**Trader**

Base contract for every trader contract (a contract that can execute ERC20 swaps). [See details](https://docs.mellow.finance/mellow-permissionless-vaults/api#trader).

### External calls made by our contracts:

- Aave
  - LendingPool: `deposit`, `withdraw`, `getReserveData`
  - aTokens: `balanceOf`
- Uniswap
  - Router: `exactInput`, `exactOutput`
  - NonfungiblePositionManager: `increaseLiquidity`, `decreaseLiquidity`, `collect`, `positions`
- Yearn
  - Yearn Vault Registry: `latestVault`
  - yTokens: `deposit`, `withdraw`, `balanceOf`

## How we protect the protocol 🔐

VaultRegistry mints a unique ERC721 NFT for each Vault. Access control is based on that NFTs:

1. Nft Owner can freely push and pull liquidity from the vault
2. Nft approved person can push, but pull only to other vaults which are in the same [Vault System](https://docs.mellow.finance/mellow-permissionless-vaults/definitions#vault-system)
3. ERC-721 ApprovedForAll cannot do anything (i.e. irrelevant to access control)

Additionally Protocol Governance admin can perform certain tasks on protocol management and emergency shutdown:

1. Disable / migrate strategies (by changing approve rights for Nfts in VaultRegistry)
2. Set strategy and protocol params on VaultGovernance level, incl setting deposit limits to 0
3. Reclaiming tokens that are sent by mistake on vaults

## Known trade-offs in the current design 🎚️

## Preemptive questions and answers ❓

## Other notes and thoughts ✍️

**External Risks**

## Setup

See Contracts [README.md]()

## How to run the tests

<div align="center">
     <h1>WEB3, CRYPTOCURRENCIES and NFT resources for OSINT investigations</h1>
     <img alt="GitHub stars" src="https://img.shields.io/github/stars/aaarghhh/awesome_osint_blockchain_analysis">
     <img alt="GitHub forks" src="https://img.shields.io/github/forks/aaarghhh/awesome_osint_blockchain_analysis"> <br>
     <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat">
     <img src="https://cdn.jsdelivr.net/gh/sindresorhus/awesome@d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg">
     <img src="https://img.shields.io/badge/Made%20With-Love-orange.svg">
     <br>
     <br>
</div>

A collection of resources useful for OSINT Investigations on Cryptocurrencies and WEB3. For sure, it isn't a complete resource, most of what you find here is related to some investigation I did. Feel free to fork and make any addition you want.


## Table of contents
- [OPSEC](#crypto-opsec-methodologies-and-info)
- [INVESTIGATION PLATFORMS AND MULTICHAIN EXPLORERS](#investigation-platforms-and-multichain-explorers)
- [SANCTIONS AND ADDRESS LABELS](#sanctions-and-address-labels)
- [SCAM AND PHISHING BLACKLISTS](#scam-and-phishing-blacklists)
- [BITCOIN](#-bitcoin---btc)
    - [Format](#btc-address-regex)
    - [Explorer](#btc-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#btc-blockchain-databases-and-analyzers)
    - [API](#btc-api)
    - [Other](#btc-other)
- [ETHEREUM](#-ethereum---eth)
    - [Format](#eth-address-regex)
    - [Explorer](#eth-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#eth-blockchain-databases-and-analyzers)
    - [Other](#eth-other)
- [OTHER EVM CHAINS](#other-evm-chains)
- [TRON](#-tron---trx)
    - [Format](#trx-address-regex)
    - [Explorer](#trx-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#trx-blockchain-databases-and-analyzers)
    - [API](#trx-api)
- [MONERO](#-monero---xmr)
    - [Format](#xmr-address-regex)
    - [Explorer](#xmr-blockchain-explorers)
- [CARDANO](#-cardano---ada)
    - [Format](#ada-address-regex)
    - [Explorer](#ada-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#ada-blockchain-databases-and-analyzers)
- [SOLANA](#-solana---sol)
    - [Format](#sol-address-regex)
    - [Explorer](#sol-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#sol-blockchain-databases-and-analyzers)
    - [Other](#sol-other)
- [TONCOIN](#-toncoin---ton)
    - [Format](#ton-address-regex)
    - [Explorer](#ton-blockchain-explorers)
    - [Other](#ton-other)
    - [API](#ton-api)
- [OTHER CHAINS (LTC, DOGE, XRP)](#other-chains-ltc-doge-xrp)
- [CROSS-CHAIN AND BRIDGE EXPLORERS](#cross-chain-and-bridge-explorers)
- [SMARTCONTRACTS](#smartcontracts)
- [DEFI](#defi)
- [NFT](#nft)
    - [NFT Databases and Analyzers](#nft-databases-and-analyzers)
    - [API](#nft-api)
- [IPFS](#ipfs)
- [METAVERSE - WEB3](#metaverse---web3)
- [DORK](#dork)
- [NOTABLE ACCOUNTS TO FOLLOW](#notable-accounts-to-follow)
- [TOOLS](#tools)
- [RESOURCES, REFERENCES, READING](#-resources-references-reading)

### CRYPTO-OPSEC Methodologies and Info
| Info / Tool | Description |
| --- | --- |
| [OfficerCIA Guide](https://github.com/OffcierCia/Crypto-OpSec-SelfGuard-RoadMap) | Collection and discussion about the best DeFi, Blockchain and crypto-related OpSec researches |
| [Anubitux](https://github.com/AnuBitux-project/build) | AnuBitux is a free project that aims to provide everyone with a safe and secure environment to manage crypto-stuff. Full documentation and tutorials [here](https://anubitux.org/). |
| [Slowmist Blockchain Darkforest](https://github.com/slowmist/Blockchain-dark-forest-selfguard-handbook) | Blockchain dark forest selfguard handbook: Master these, master the security of your cryptocurrency. |

## INVESTIGATION PLATFORMS AND MULTICHAIN EXPLORERS
| Link | Description |
| --- | --- |
| [MistTrack](https://misttrack.io/) | AML tracing and risk detection platform by SlowMist, it has a free tier and supports BTC, ETH, TRON, BSC and many other chains |
| [Bubblemaps](https://v2.bubblemaps.io/) | Visualizes token holders as clusters of connected wallets, very useful to spot insiders, sybil wallets and rug pulls |
| [Nansen](https://nansen.ai/) | Onchain analytics platform with millions of labeled wallets ("smart money", funds, exchanges) |
| [Arkhamintelligence](https://platform.arkhamintelligence.com) | Entity attribution and network mapping across many chains (BTC, ETH, TRON, SOL, EVM L2s and others) |
| [Blockscan](https://blockscan.com/) | Search an address across all the Etherscan-family EVM explorers at once |
| [OKLink](https://www.oklink.com/) | Multichain explorer with address labels, it supports BTC, ETH, TRON, BSC, Polygon, L2s and many others |
| [Hopchain](https://hopchain.io/) | Free, no-signup counterparty graph of an address with known-entity labels and scam/sanction flags, plus a Sybil/cluster check for up to 50 addresses. It supports EVM chains, TRON and Solana (no BTC) |
| [PublicAML](https://publicaml.org) | Free, no-signup AML screening of BTC, ETH, BNB Chain and TRON addresses: risk score, OFAC/EU sanctions status, category and source of funds. Free API available. [Anonymous operator, use as a hint not as evidence] |
| [Chainalysis](https://www.chainalysis.com/) | Commercial blockchain analytics (Reactor, KYT), the de-facto standard for law enforcement investigations |
| [Elliptic](https://www.elliptic.co/) | Commercial blockchain analytics and crypto compliance platform (Investigator, Lens, Navigator) |
| [Merkle Science](https://www.merklescience.com/) | Commercial crypto risk and intelligence platform (Tracker, Compass) |

## SANCTIONS AND ADDRESS LABELS
| Link | Description |
| --- | --- |
| [OFAC Sanctions Search](https://sanctionssearch.ofac.treas.gov/) | The official US Treasury SDN search, sanctioned entities often include their crypto addresses |
| [OFAC sanctioned addresses](https://github.com/0xB10C/ofac-sanctioned-digital-currency-addresses) | Daily extraction of the crypto addresses in the OFAC SDN list, split in one file per chain |
| [OpenSanctions](https://www.opensanctions.org/) | Open database of sanctions, PEPs and watchlists, it includes crypto wallets |
| [eth-labels](https://github.com/dawsbot/eth-labels) | A public dataset of labeled crypto addresses (EVM chains) |
| [etherscan-labels](https://github.com/brianleect/etherscan-labels) | Full label data dump of the top EVM explorers in JSON/CSV |

## SCAM AND PHISHING BLACKLISTS
| Link | Description |
| --- | --- |
| [ScamSniffer scam-database](https://github.com/scamsniffer/scam-database) | Web3 blacklists (domains and addresses) maintained by Scam Sniffer |
| [MetaMask eth-phishing-detect](https://github.com/MetaMask/eth-phishing-detect) | The phishing domains blocklist used by MetaMask |
| [SEAL - Security Alliance](https://securityalliance.org/) | Security researchers alliance, SEAL 911 helps during ongoing hacks and drains |
| [Chainabuse](https://www.chainabuse.com/) | Community scam reports on addresses and domains, multichain |

## <img src="https://cryptologos.cc/logos/bitcoin-btc-logo.png" alt="btc" style="width:25px;" width="25" height="25" /> Bitcoin - BTC

### BTC Address Regex
| Address regex | Description |
| --- | --- |
| `1[a-km-zA-HJ-NP-Z1-9]{25,34}` | Legacy addresses |
| `3[a-km-zA-HJ-NP-Z1-9]{25,34}` | P2SH address |
| `bc1[qpzry9x8gf2tvdw0s3jn54khce6mua7l]{39,59}` | Segwit addresses |
| `bc1p[qpzry9x8gf2tvdw0s3jn54khce6mua7l]{59}` | Taproot addresses |

### BTC Blockchain explorers
| Link | Description |
| --- | --- |
| [3xpl.com](https://3xpl.com/bitcoin) | Fastest ad-free universal block explorer |
| [Blockchain.com](https://www.blockchain.com/explorer/assets/btc) | One of the first and most robust explorers, it permits to explore Bitcoin, Ethereum, Bitcoin Cash, other assets and also NFT |
| [Blockchair](https://blockchair.com/bitcoin) | An explorer that supports different cryptocurrencies, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block |
| [Crystal Intelligence (Lite)](https://lite.crystalintelligence.com/) | The public explorer (formerly Crystalblockchain) helps to search for addresses and transactions, it also displays comprehensive details about an address. |
| [Tokenview](https://tokenview.io/) | Another blockchain explorer, it supports different tokens and cryptocurrencies, BTC, ETH, XMR ... Search info by addresses and/or transactions |
| [Graphsense](https://graphsense.org/) | GraphSense is a cryptoasset analytics platform emphasizing full data sovereignty, algorithmic transparency, and scalability. |
| [Coincodex](https://coincodex.com/crypto/bitcoin/historical-data/) | Historical price of Bitcoin |
| [Awebanalysis](https://awebanalysis.com/en/bitcoin-address-validate/) | Validate Bitcoin format |
| [WalletExplorer](https://www.walletexplorer.com/) | A service which tries to retrieve the wallet related to an address [#BecarefulwhatyouOSINTWith](https://www.theblock.co/news/regulation/2021-09-21-chainalysis-used-an-ip-scraping-block-explorer-to-aid-law-enforcement-leaked-docs-say-118223) |
| [Breadcrumbs.app](https://www.breadcrumbs.app/) | An investigation tool that helps to visualize address relations, it's very helpful and it contains information about sanctioned addresses and assets. It supports BTC, ETH and any ERC20 Token |
| [TRM](https://www.trmlabs.com/) | TRM Transaction Monitor and TRM Forensics are two tools that help in depth analysis on Blockchain transactions |
| [Lampyre](https://lampyre.io/) | Like Maltego it supports BTC investigations and correlations. |
| [Bitquery.io](https://www.bitquery.io/) | Full explorer which supports addresses analysis, smartcontracts and assets explorer |
| [Whalealert](https://whale-alert.io/) | An alerting system, it's helpful to get alerts when wallets with a big amount of funds are making transactions |
| [BTCparser](https://btcparser.com/) | A project to get information about different kinds of wallets, it monitors old wallets or wallets related to the Satoshi era |
| [Bitref](https://bitref.com) | A simple address explorer. It displays the amount of Bitcoin held on given addresses |
| [Arkhamintelligence](https://platform.arkhamintelligence.com) | Entity attribution and network mapping, it supports BTC and many other chains |
| [Metasleuth](https://metasleuth.io/) | BTC Address explorer and wallet monitor |
| [Blockstream.info](https://blockstream.info/) | Open-source Bitcoin explorer by Blockstream, also available as Tor hidden service |
| [Ordiscan](https://ordiscan.com/) | Explorer for Bitcoin Ordinals inscriptions and Runes |

### BTC Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Bitcoinwho'swho](https://www.bitcoinwhoswho.com/) | An address lookup service to identify reports related to malicious BTC addresses. |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA. It also incorporates the former Bitcoinabuse database |
| [Scamsearch](https://www.scamsearch.io/) | It's a global scam database. Search by Profile Picture, Email, Username, Pseudo Name, Phone Number, crypto address or website. |
| [Scamalert](https://scam-alert.io/) | It offers a search engine for scam and crypto-address related frauds |
| [Cryptoscamdb](https://cryptoscamdb.org/scams) | A scam database which contains information about scam sites and related addresses |
| [Ransomwhere](https://ransomwhe.re/) | Bitcoin addresses used in ransomware activities, the database is in raw format and it's integrated in the Chainabuse service |
| [SPLcenter Addresslist](https://www.splcenter.org/resources/reports/cryptocurrency-report/) | A spreadsheet containing information about addresses used by extremists and far right communities |

### BTC API
| Req | Description |
| --- | --- |
| `https://3xpl.com/bitcoin/address/xxx` | Request for the status of the address using 3xpl API |
| `https://blockchair.com/bitcoin/address/xxx` | Request for the status of the address using Blockchair API |
| `https://blockchair.com/bitcoin-cash/transaction/xxx` | Request for the detail of a given transaction |
| `https://blockchain.info/q/24hrprice` | Retrieving the price of the last 24h |
| `https://blockchain.info/q/getreceivedbyaddress/xxx` | Retrieving the amount received on a given BTC address |
| `https://blockchain.info/q/getsentbyaddress/xxx` | Retrieving information of what was sent by a given address |
| `https://blockchain.info/q/addressbalance/xxx` | Retrieving the balance for a given address |
| `https://blockchain.info/q/addressfirstseen/xxx` | It retrieves the first seen date of a given address |

### BTC Other
| Link | Description |
| --- | --- |
| [CriminalIP](https://search.criminalip.io/asset/search?query=%22Bitcoin%22%20port:%208333) | It's an infrastructure scanner. It scans IPs and services, there is a section related to miner services exposed online |
| [Intelx.io](https://intelx.io/) | It indexes information retrieved from both closed and open sources. It also indexes IP, email, BTC addresses and other kinds of assets |
| [Cryptocurrencyalerting](https://cryptocurrencyalerting.com/wallet-watch.html) | Getting alerts about transactions related to a given address |
| [Aware Online](https://www.aware-online.com/en/osint-tools/cryptocurrency-search-tool/) | Different tools to conduct OSINT investigations on given BTC addresses |
| [GraphSense Maltego Transform](https://github.com/INTERPOL-Innovation-Centre/GraphSense-Maltego-transform) | A Maltego transform which leverages the power of GraphSense for Crypto investigations |
| [Mempool Space](https://mempool.space/) | A graphical dashboard to analyze the history of block congestion, fees, lightning network and mining activities |
| [Amboss](https://amboss.space/) | Lightning Network explorer, useful to profile nodes, aliases and channels |
| [1ML](https://1ml.com/) | Lightning Network search and analysis engine, nodes are searchable by alias and IP |

## <img src="https://cryptologos.cc/logos/ethereum-eth-logo.png" alt="eth" style="width:25px;" width="25" height="25" /> Ethereum - ETH

### ETH Address Regex
| Address regex | Description |
| --- | --- |
| `0x[0-9A-Fa-f]{40}` | All Ethereum addresses have a length of 40 hexadecimal characters and begin with “0x”. The same format is used by every EVM chain (BSC, Polygon, Base, Arbitrum ...), so the same address can be active on more chains |

### ETH Blockchain explorers
| Link | Description |
| --- | --- |
| [3xpl.com](https://3xpl.com/ethereum) | Fastest ad-free universal block explorer. |
| [Blockchain.com](https://www.blockchain.com/explorer/assets/eth) | One of the first and most robust explorers, it permits to explore Bitcoin, Ethereum, Bitcoin Cash, other assets and also NFT |
| [Etherscan](https://etherscan.io/) | The most reliable and complete explorer for the Ethereum ecosystem. It helps to search addresses, tokens, NFTs, smartcontracts and also ENS domains |
| [Blockchair](https://blockchair.com/ethereum) | An explorer that supports different cryptocurrencies, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block |
| [Tokenview](https://tokenview.io/) | Another blockchain explorer, it supports different tokens and cryptocurrencies, BTC, ETH, XMR ... Search info by addresses and/or transactions |
| [Blockscout](https://eth.blockscout.com/) | It covers all about Ethereum, from transactions and block information, token values to sidechains and private chains |
| [Ethtective](https://ethtective.com/) | It has a very interesting way to visualize the Ethereum network, that makes exploring transfers much more interactive. |
| [Graphsense](https://graphsense.org/) | GraphSense is a cryptoasset analytics platform emphasizing full data sovereignty, algorithmic transparency, and scalability. |
| [BitQuery](https://explorer.bitquery.io/ethereum) | A Blockchain explorer which supports different kinds of assets. It supports BTC, ETH, DOGE, ADA etc |
| [Ethplorer](https://ethplorer.io/) | Track address portfolios for any Ethereum address with comprehensive balance charts and transactions |
| [ENS Domains](https://app.ens.domains/) | An ENS domain explorer, mainly used to purchase that kind of asset, it also helps to find ENS domains and related information |
| [Unstoppable Domains](https://unstoppabledomains.com/) | Registrar and marketplace for web3 domains (.crypto, .nft, .x ...), useful to resolve them to wallet addresses |
| [Breadcrumbs.app](https://www.breadcrumbs.app/) | An investigation tool that helps to visualize address relations, it's very helpful and it contains information about sanctioned addresses and assets. It supports BTC, ETH and any ERC20 Token |
| [Arkhamintelligence](https://platform.arkhamintelligence.com) | Entity attribution and network mapping, it supports ETH, EVM L2s and many other chains |
| [Watchers.pro](https://watchers.pro) | [Warning!!! Create a sock wallet, it needs a Metamask extension to access it] A tool that provides a dashboard for clustering and inspecting DEFI and altcoin related entities |
| [Metasleuth](https://metasleuth.io/) | ETH Address explorer and wallet monitor |
| [TrackEnn](https://github.com/kennbroorg/trackenn) | Traceability project in blockchain. Ethereum for now. Transactions, internals, ERC-20 transfers, contracts, internal tagging, labeling, etc |
| [Ward Graph](https://github.com/WardAnalytics/WardGraph) | Nice open-source graph explorer for ETH blockchain |
| [Socketscan](https://www.socketscan.io/) | EVM bridge explorer |

### ETH Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA |
| [Scamsearch](https://www.scamsearch.io/) | It's a global scam database. Search by Profile Picture, Email, Username, Pseudo Name, Phone Number, crypto address or website. |
| [Cryptoscamdb](https://cryptoscamdb.org/scams) | A scam database which contains information about scam sites and related addresses |
| [SPLcenter Addresslist](https://www.splcenter.org/resources/reports/cryptocurrency-report/) | A spreadsheet containing information about addresses used by extremists and far right communities |
| [Walletlabels](https://www.walletlabels.xyz/) | Search engine based on a collection of more than 7.5M ETH labeled addresses |
| [Dune](https://dune.com/discover/content/trending) | A community driven dashboards collection, useful for exploring ETH, TOKENS and NFT |

### ETH Other
| Link | Description |
| --- | --- |
| [Chat Blockscan](https://chat.blockscan.com/) | A chat based on Ethereum blockchain, useful to reach an ENS domain or address owner |
| [Bluepages.fyi](https://bluepages.fyi) | Address ↔ social identity lookup: maps X/Twitter and Farcaster accounts to crypto addresses (6M+ addresses) and searches tweets mentioning an address. Pay-per-query (USDC on Base) or prepaid API key |
| [CriminalIP](https://search.criminalip.io/asset/search?query=%22Ethereum%22%20port:%208545) | It's an infrastructure scanner. It scans IPs and services, there is a section related to miner services exposed online |
| [Naddison36](https://github.com/naddison36/tx2uml) | Ethereum transaction to UML sequence diagram generator |
| [Cryptocurrencyalerting](https://cryptocurrencyalerting.com/wallet-watch.html) | Getting alerts about transactions related to a given address |
| [Aware Online](https://www.aware-online.com/en/osint-tools/cryptocurrency-search-tool/) | Different tools to conduct OSINT investigations on given ETH addresses |
| [GraphSense Maltego Transform](https://github.com/INTERPOL-Innovation-Centre/GraphSense-Maltego-transform) | A Maltego transform which leverages the power of GraphSense for Crypto investigations |
| [Etherscan Transforms for Maltego](https://www.maltego.com/transform-hub/etherscan/) | The official Etherscan transform for Maltego |
| [Demixing Tornado cash bot](https://flipsidecrypto.xyz/AMLBot/demixin-eth-for-tornadocash-JCcIiS) | Tool for demixing transactions made using Tornado cash (updated weekly) |
| [Cielo](https://app.cielo.finance/) | A tool for tracking and monitoring EVM wallets |
| [Phalcon Explorer](https://blocksec.com/phalcon/explorer) | Transaction analysis by BlockSec: fund flows, call traces and balance changes, very useful for hacks and exploits |
| [Tenderly](https://tenderly.co/) | Transaction debugger and simulator, it shows the full execution trace of an EVM transaction |

## OTHER EVM CHAINS
| Link | Description |
| --- | --- |
| [BscScan](https://bscscan.com/) | The reference explorer for BNB Smart Chain |
| [Polygonscan](https://polygonscan.com/) | The reference explorer for Polygon PoS |
| [Basescan](https://basescan.org/) | The reference explorer for Base (Coinbase L2) |
| [Arbiscan](https://arbiscan.io/) | The reference explorer for Arbitrum One |
| [Blockscan](https://blockscan.com/) | Search an address across all the Etherscan-family EVM explorers at once |

## <img src="https://cryptologos.cc/logos/tron-trx-logo.png" alt="trx" style="width:25px;" width="25" height="25" /> Tron - TRX

### TRX Address Regex
| Address regex | Description |
| --- | --- |
| `T[1-9A-HJ-NP-Za-km-z]{33}` | Base58 address of 34 characters starting with 'T'. TRON is the main network for USDT (TRC20) transfers, widely abused by scams and money laundering |

### TRX Blockchain explorers
| Link | Description |
| --- | --- |
| [Tronscan](https://tronscan.org/) | The official TRON explorer, it shows addresses, transactions, TRC20 transfers and address tags |
| [OKLink](https://www.oklink.com/tron) | Multichain explorer with address labels, it supports TRON |
| [Blockchair](https://blockchair.com/tron) | An explorer that supports different cryptocurrencies, it also supports TRON |

### TRX Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [MistTrack](https://misttrack.io/) | AML tracing and risk detection with address labels, it supports TRON and USDT-TRC20 flows |
| [Chainabuse](https://www.chainabuse.com/) | Community scam reports, it supports TRON addresses |
| [TRON Checker](https://usdt.chikocorp.com/tron-usdt-blacklist-checker) | Free, no-signup check of a TRON address against Tether's USDT-TRC20 blacklist (direct contract read cross-checked with TronScan) and the OFAC SDN list, with timestamps and explainable risk indicators. API available |

### TRX API
| Req | Description |
| --- | --- |
| `https://api.trongrid.io/v1/accounts/xxx` | Retrieving the account details (balance, TRC20 balances, permissions) of a given address using TronGrid |
| `https://api.trongrid.io/v1/accounts/xxx/transactions/trc20?limit=200` | Retrieving the TRC20 (e.g. USDT) transfers of a given address |

## <img src="https://cryptologos.cc/logos/monero-xmr-logo.png" alt="xmr" style="width:25px;" width="25" height="25" /> Monero - XMR

### XMR Address Regex
| Address regex | Description |
| --- | --- |
| `[48][1-9A-HJ-NP-Za-km-z]{94}` | A raw Monero address is a set of 95 base58 characters starting with a '4' or an '8' |

### XMR Blockchain Explorers
| Link | Description |
| --- | --- |
| [Blockchair](https://blockchair.com/monero) | Helps to inspect transactions and related hashes. |
| [xmrchain.net](https://xmrchain.net/) | Open-source Monero explorer, it can decode outputs given an address and a view key, and prove payments with a tx key |

## <img src="https://cryptologos.cc/logos/cardano-ada-logo.png" alt="ada" style="width:25px;" width="25" height="25" /> Cardano - ADA

### ADA Address Regex
| Address regex | Description |
| --- | --- |
| `Ae2[1-9A-HJ-NP-Za-km-z]+` | Legacy address ( Byron ) - Icarus-style |
| `DdzFF[1-9A-HJ-NP-Za-km-z]+` | Legacy address ( Byron ) - Daedalus-style |
| `addr1[a-z0-9]+` | Shelley address |
| `stake1[a-z0-9]+` | Shelley address used in staking pool |

### ADA Blockchain explorers
| Link | Description |
| --- | --- |
| [Blockchain.com](https://www.blockchain.com/explorer/assets/ada) | One of the first and most robust explorers, it permits to explore Bitcoin, Ethereum, Bitcoin Cash, other assets and also NFT |
| [Cardano explorer](https://explorer.cardano.org/) | The official scanner for Cardano transactions, it helps to analyze addresses, transactions for each epoch |
| [Blockchair](https://blockchair.com/cardano) | An explorer that supports different cryptocurrencies, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block. |
| [Adastat](https://adastat.net/) | An explorer related to the whole Cardano ecosystem, it can inspect Addresses, Blocks, Transactions, Epochs |
| [Cexplorer](https://cexplorer.io/) | A staking pool explorer (formerly Adapools), it helps to browse staking pools and their current activities |
| [BitQuery](https://www.bitquery.io/) | Full explorer which supports addresses analysis, smartcontracts and assets explorer |

### ADA Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA |

## <img src="https://cryptologos.cc/logos/solana-sol-logo.png" alt="sol" style="width:25px;" width="25" height="25" /> Solana - SOL

### SOL Address Regex
| Address regex | Description |
| --- | --- |
| `[1-9A-HJ-NP-Za-km-z]{32,44}` | A Solana address's length varies from 32 to 44 characters. |

### SOL Blockchain explorers
| Link | Description |
| --- | --- |
| [Solana Explorer](https://explorer.solana.com/) | The official scanner for Solana transactions, it helps to analyze addresses, transactions, tokens |
| [Blockchair](https://blockchair.com/solana) | An explorer that supports different cryptocurrencies, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block. |
| [Solscan.io](https://solscan.io/) | A Solana scanner which supports Address, transaction, token and NFT. Solscan was acquired by Etherscan |
| [SolanaFM](https://solana.fm/) | Solana explorer with human readable transaction decoding and address labels |
| [Birdeye](https://birdeye.so/) | Token and DEX trading analytics for Solana (and other chains), useful to inspect traders and token launches |

### SOL Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA |

### SOL Other
| Link | Description |
| --- | --- |
| [SNS - Solana Name Service](https://www.sns.id/) | Resolve `.sol` domains to wallet addresses and vice versa |

## <img src="https://cryptologos.cc/logos/toncoin-ton-logo.png" alt="ton" style="width:25px;" width="25" height="25" /> Toncoin - TON

### TON Address Regex
| Address regex | Description |
| --- | --- |
| `0:[a-f0-9]{64}` | The raw address, it is in hexadecimal format |
| `(E\|U)Q[a-zA-Z0-9\-\_]{46}` | Friendly name, based on a custom hash algorithm, ref: crc16 custom, some insight on different kinds of [Wallets](https://docs.ton.org/contracts/standard/wallets/comparison). |
| `\w\s\w\s\w` | It also supports generated nicknames like `Graceful Tan Takin` <_< |

### TON Blockchain explorers
| Link | Description |
| --- | --- |
| [3xpl.com](https://3xpl.com/ton) | Fastest ad-free universal block explorer |
| [Tonviewer](https://tonviewer.com/) | The main TON explorer (by Tonkeeper), it shows addresses, jettons, NFTs, domains and decoded transaction traces |
| [Tonscan](https://tonscan.org/) | An address lookup service, it helps to find details about a given address |
| [Toncoin](https://explorer.toncoin.org/) | A more technical explorer, it helps to query the TON network using different key fields, workchain, shard and so on |
| [TonAPI](https://tonapi.io/api-v2) | A platform and API useful to inspect TON addresses and any related assets, it supports Numbers and also NFT |
| [GetGems](https://getgems.io/top-collections) | A marketplace for NFTs for TON network assets |

### TON Other
| Link | Description |
| --- | --- |
| [Fragment](https://fragment.com/numbers) | A marketplace / auction used to purchase numbers or nicknames usable on the Telegram platform `https://fragment.com/username/[username]` |
| [Ton place](https://ton.place/) | A platform to monetize content and fanbase, dork `site:ton.place [content]` |
| [Tonex](https://tonex.app/) | A social network directly integrated on TON network |
| [TONwhale](https://tonwhales.com/explorer/top) | A list of top 1000 accounts |
| [ATOP](https://github.com/aaarghhh/a_TON_of_privacy) | A tool to make investigations on TON NFTs like Telegram fake numbers, Telegram nicknames, and TON domains. |
| [TON Forbes](https://tonforbes.com) | TON Forbes is an intelligent social rating of The Open Network blockchain wallets. |

### TON API
| Link | Description |
| --- | --- |
| Get bulk info about some addresses | `curl -X 'POST' 'https://tonapi.io/v2/accounts/_bulk' -H 'Content-Type: application/json' -d '{"account_ids":["0:da6b1b6663a0e4d18cc8574ccd9db5296e367dd9324706f3bbd9eb1cd2caf0bf"]}'` |
| Get info about a TON domain | `curl -X 'GET' 'https://tonapi.io/v2/dns/wallet.ton' -H 'accept: application/json'` |
| Search all Telegram numbers (paginated) | `curl -X 'GET' 'https://tonapi.io/v2/nfts/collections/0:0e41dc1dc3c9067ed24248580e12b3359818d83dee0304fabcf80845eafafdb2/items?limit=100&offset=0' -H 'accept: application/json'` |
| Get a backresolve of a domain | `curl -X 'GET' 'https://tonapi.io/v2/accounts/0:BA60BFBD527C0CD2D70C6396630C50A498AF015B987ADAAD1D4A9E287F604536/dns/backresolve' -H 'accept: application/json'` |
| Get current bids for a domain | `curl -X 'GET' 'https://tonapi.io/v2/dns/wallet.ton/bids' -H 'accept: application/json'` |
| Retrieve data from a given NFT | `https://ton.diamonds/api/v1/explorer/search_list` |

## OTHER CHAINS (LTC, DOGE, XRP)
| Address regex | Description |
| --- | --- |
| `[LM][a-km-zA-HJ-NP-Z1-9]{26,33}` | Litecoin legacy (L) and P2SH (M) addresses |
| `ltc1[qpzry9x8gf2tvdw0s3jn54khce6mua7l]{39,59}` | Litecoin Segwit addresses |
| `D[5-9A-HJ-NP-U][1-9A-HJ-NP-Za-km-z]{32}` | Dogecoin addresses |
| `r[1-9A-HJ-NP-Za-km-z]{24,34}` | XRP Ledger classic addresses |

| Link | Description |
| --- | --- |
| [Litecoin Space](https://litecoinspace.org/) | Litecoin explorer based on mempool.space |
| [Dogechain](https://dogechain.com/) | Dogecoin block explorer |
| [XRPSCAN](https://xrpscan.com/) | XRP Ledger explorer with account names and labels |
| [Blockchair](https://blockchair.com/) | It also supports Litecoin, Dogecoin and XRP |

## CROSS-CHAIN AND BRIDGE EXPLORERS
| Link | Description |
| --- | --- |
| [Range](https://explorer.range.org/) | Cross-chain explorer, it supports CCTP transactions |
| [Socketscan](https://www.socketscan.io/) | EVM bridge explorer |
| [LayerZero Scan](https://layerzeroscan.com/) | Explorer for LayerZero cross-chain messages, useful to follow funds bridged through Stargate and other OApps |
| [Wormholescan](https://wormholescan.io/) | Explorer for Wormhole bridge transfers (EVM, Solana, Sui ...) |
| [Axelarscan](https://axelarscan.io/) | Explorer for Axelar cross-chain transfers |

## SMARTCONTRACTS
| Tool | Description |
| --- | --- |
| [Ethereum Signature Database](https://www.4byte.directory/) | A database containing the bytes signatures related to functions used in smartcontracts |
| [Sourcify 4byte](https://4byte.sourcify.dev/) | Another function and event signature database (the successor of openchain.xyz) |
| [Grep.app](https://grep.app/search?q=solidity) | Search for smartcontract source code. It could be useful to search for NFT or contract source code |
| [EIS3](https://github.com/salaheldinaz/EIS3) | An ENS domain (.eth domain) analyzer |
| [Dune](https://dune.com/discover/content/trending) | A community driven dashboards collection, useful for exploring ETH, TOKENS and NFT |

## DEFI
| Link | Description |
| --- | --- |
| [DexScreener](https://dexscreener.com/) | Real-time DEX pairs tracker on many chains, useful to find token deployers and early traders |
| [GeckoTerminal](https://www.geckoterminal.com/) | DEX tracker by CoinGecko, it shows pools, trades and liquidity |
| [DefiLlama](https://defillama.com/) | TVL, protocols and hacks dashboard, it keeps a list of DeFi hacks |
| [Rekt.news](https://rekt.news/) | Post-mortems and leaderboard of the biggest DeFi hacks and exploits |
| [Token Terminal](https://tokenterminal.com/) | Financial and onchain fundamentals of crypto protocols |

## NFT
| Tool | Description |
| --- | --- |
| [Opensea](https://opensea.io/) | The first and most relevant NFT marketplace, it also supports ENS names, accounts can be explored using this pattern: `https://opensea.io/[nickname]` |
| [Binance NFT](https://www.binance.com/en/nft/) | NFT marketplace directly managed by Binance |
| [Blur](https://blur.io/) | NFT marketplace and aggregator for Ethereum, focused on pro traders |
| [Magic Eden](https://magiceden.io/) | Multichain NFT marketplace (Solana, Bitcoin Ordinals, Ethereum and others) |
| [CryptoSlam](https://cryptoslam.io/) | NFT sales data, rankings and collection statistics |
| [Rarible](https://rarible.com/) | Another NFT marketplace, it supports ETH, SOL, Tezos and Polygon |
| [Crypto.com](https://crypto.com/nft) | NFT marketplace directly managed by Crypto.com |
| [NFT Calendar](https://nftcalendar.io/) | A Calendar for NFT projects, it doesn't require any author validation |
| [NFTfinder](https://www.nyckel.com/nft-finder) | A reverse search for finding NFTs, it supports images, addresses and so on |
| [NFT Analyst Starter Pack](https://github.com/a16z/nft-analyst-starter-pack) | Using an Alchemy API key, it can generate CSV extracts for all token transfers, historical sales, and each underlying item's metadata |
| [Tonnft](https://explorer.tonnft.tools/) | A marketplace and explorer for TON NFTs |
| [GetGems](https://getgems.io/top-collections) | Another marketplace for NFTs for TON network assets |
| [NFTGO.io](https://nftgo.io/) | Discover, analyze, and trade NFTs faster and smarter than anyone else, aided by in-depth analytics and intelligent toolkits. |
| [NFT scan](https://www.nftscan.com/) | An NFT explorer which supports different blockchains like Ethereum, Binance, Polygon, Solana and others |
| [Dune](https://dune.com/discover/content/trending) | A community driven dashboards collection, useful for exploring ETH, TOKENS and NFT |
| [ZORA](https://zora.co/collect/eth:0x054460490780a6eb15625d703db1754e0b78d846) | A platform for minting NFTs, it lets you explore useful information on some MINT statistics |

### NFT Databases and Analyzers
| Link | Description |
| --- | --- |
| [Scamsniffer](https://explorer.scamsniffer.io/?sort=30DayVolume) | A full solution to track NFT scammers, it also supports a Browser extension and a Discord bot |

### NFT API
| Tool | Description | API CALL |
| --- | --- | --- |
| [Alchemy API](https://www.alchemy.com/nft-api) | Helps to navigate ETH and other chain data via API | `import { Alchemy } from "alchemy-sdk";Alchemy().nft.getNftsForOwner("0xshah.eth").then(console.log);` |

## IPFS
| Tool | Description |
| --- | --- |
| `ipfs dht findprovs <hash-of-file>` | Returns IDs of all nodes having the file |
| `ipfs dht findpeer <nodeID>` | Returns the list of node addresses (IP v4 and v6, TCP and UDP) |
| [IPFS scanner](https://github.com/cryptodashie/ipfs/tree/fda709851b21d9ef82eb246da6f96667f14f3ae8) | IPFS scanning can identify new hosted content or expose information leaks similar to Amazon S3 buckets. |
| [IPFS browser](https://ipfsbrowser.com/) | Search, view, access, and download IPFS files quickly and easily right in your web browser from any device! |

## METAVERSE - WEB3
| Link | Description |
| --- | --- |
| [Spatial](https://www.spatial.io) | An example of Metaverse, it contains different spaces where people can connect with. `https://www.spatial.io/@[USERNAME]` |
| [Debank](https://debank.com/) | A WEB3 messenger and Portfolio |
| [Zapper](https://zapper.xyz/) | A multichain WEB3 explorer. It allows to search and monitor different kinds of assets like TOKEN, NFT etc. |
| [Scamsniffer](https://www.scamsniffer.io/extension/) | A Chrome extension aimed to block and detect scams and rugpulls during WEB3 surfing |

## DORK
| Dork | Description |
| --- | --- |
| `[ADDRESS] -block` | Identify information related to the address but not indexed by common search engines |
| `site:[url of interest] [ADDRESS]` | Helps to find information about an address on a target url of interest |
| `(antminer) AND protocols.raw: “80/http” AND 80.http.get.title: “401”` | (Shodan) dork for antminer |
| `ETH - Total Speed` | (Shodan) Claymore Miner Software |

## NOTABLE ACCOUNTS TO FOLLOW
| Account | Description |
| --- | --- |
| [CIA_Officer](https://x.com/officer_secret) | Independent Security Researcher • Not the CIA • OpSec & Privacy Guru • On-Chain & OSINT Sleuth |
| [Rugpullfinder (Inactive)](https://x.com/rugpullfinder) | The NFT community's premier source of information |
| [ZachXBT](https://x.com/zachxbt) | On-chain sleuth. Rug pull survivor turned 2D detective |
| [Tay](https://x.com/tayvano_) | Security researcher at MetaMask, investigations on hacks, drainers and DPRK related thefts |
| [PeckShieldAlert](https://x.com/peckshieldalert) | Real-time alerts about hacks, exploits and phishing |
| [MistTrack](https://x.com/MistTrack_io) | Alerts and fund flow analysis of hacks and scams by SlowMist |
| [Scam Sniffer](https://x.com/realScamSniffer) | Alerts and reports about phishing and wallet drainers |
| [samczsun](https://x.com/samczsun) | Security researcher, SEAL 911 founder |

## TOOLS
| Tool | Description |
| --- | --- |
| [Obsidian templates Cryptocurrencies](https://github.com/theNerdInTheHighCastle/obsidian-osint-templates/blob/main/--%20templates/Cryptocurrency%20Investigation%20Findings%20Report.md) | An Obsidian template for Cryptocurrencies investigations |
| [Obsidian templates NFT](https://github.com/theNerdInTheHighCastle/obsidian-osint-templates/blob/main/--%20templates/NFT.md) | An Obsidian template for NFT investigations |
| [Eth Explorers Extension](https://github.com/apoorvlathey/eth-explorers-extension) | Browser extension to open Ethereum addresses & transaction hashes from any page on popular explorers + dashboards |
| [Maltego](https://www.maltego.com/) | Maltego directly supports BTC and ETH address entities. It is a tool used for OSINT and Forensic investigations |
| [Tatum Blockchain Explorer (Maltego Transform)](https://www.maltego.com/) | Tatum is a blockchain development platform that supports over 40 blockchain protocols and 2000+ digital assets. |
| [Opensanctions (Maltego Transform)](https://www.maltego.com/) | A transform for Maltego, it queries sanctioned addresses from the OpenSanctions database |
| [EMER name (Maltego Transform)](https://github.com/Tomasuh/Maltego_Transform_Blockchain_DNS/tree/63e6fb152a75893103ec038b9974db937ba21baa) | Useful transform to resolve EMER domain names |
| [Mugetsu](https://t.me/the_mugetsu_bot) | Correlation from X handle, wallet identification, trading analysis and wallet explorer |
| [Impersonator](https://chromewebstore.google.com/detail/impersonator/hgihfkmoibhccfdohjdbklmmcknjjmgl) | Spoof ETH address for authenticating in Dapps |


## 📖 RESOURCES, REFERENCES, READING
| Resource | Description |
| --- | --- |
| [Cia Operator Start.me](https://cia.start.me/p/dlaxD0/ciaofficerv2) | The start.me of CIA operators, an infinite source of news and interesting tools |
| [LeHACK Video](https://www.youtube.com/watch?v=MVHHokKEp7s&t=1101s) | A great video from [LeHack](https://lehack.org/), with techniques, real examples and case-studies for ETH investigations |
| [Crypto Mindmaps](https://cryptoengineer.notion.site/cryptoengineer/9f1668632aa04a0a83a311a86e799254?v=f7c5c49231f44b91a44021411fa27e28) | Useful mindmaps related to crypto and WEB3 |
| [Tornadocash after censorship](https://hackmd.io/@gozzy/tornado-cash-post-censorship) | A guide to bypass Tornadocash censorship (note: OFAC delisted Tornado Cash in March 2025) |
| [WEB3 is going great](https://www.web3isgoinggreat.com/) | Daily news about what's going wrong on Crypto and WEB3 |
| [The Nerd in the high castle](https://thenerdinthehighcastle.wordpress.com) | OSINT and FORENSICS tutorial and articles |
| [Bellingcat Online Investigation Toolkit](https://bellingcat.gitbook.io/toolkit) | Bellingcat's catalogue of investigation tools, it also contains a section about crypto and blockchain |
| [Chainalysis Reports](https://www.chainalysis.com/reports/) | Yearly Crypto Crime Report and other research on illicit flows, [2026 edition](https://www.chainalysis.com/reports/crypto-crime-2026/) |
| [TRM Labs Crypto Crime Report](https://www.trmlabs.com/reports-and-whitepapers/2025-crypto-crime-report) | Yearly report on illicit crypto activity, other research is available in the [resources](https://www.trmlabs.com/resources) section |

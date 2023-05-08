<div align="center">
     <h1>WEB3, CRIPTOCURRENCIES and NFT resources for OSINT investigations</h1>
     <img alt="GitHub stars" src="https://img.shields.io/github/stars/aaarghhh/osint_criypto_web3_stuff"> 
     <img alt="GitHub forks" src="https://img.shields.io/github/forks/aaarghhh/osint_criypto_web3_stuff"> <br>
     <img src="https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat">
     <img src="https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg">
     <img src="https://img.shields.io/badge/Made%20With-Love-orange.svg">
     <br>
     <br>
</div>

A collection of resources useful for OSINT Investigations on Cryptocurrencies and WEB3. For sure, it isn't a complete resource, most of what you find here is related to some investigation I did. Feel free to fork and make any addition you want. 


## [](#table-of-contents) Table of contents
- [OPSEC](#crypto-opsec-methodologies-and-info)
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
- [MONERO](#-monero---xmr)
    - [Format](#xmr-address-regex)
    - [Explorer](#xmr-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#xmr-blockchain-databases-and-analyzers)
- [CARDANO](#-cardano---ada)
    - [Format](#ada-address-regex)
    - [Explorer](#ada-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#ada-blockchain-databases-and-analyzers)
- [SOLANA](#-solana---sol)
    - [Format](#sol-address-regex)
    - [Explorer](#sol-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#sol-blockchain-databases-and-analyzers)
- [TONCOIN](#-toncoin---ton)
    - [Format](#ton-address-regex)
    - [Explorer](#ton-blockchain-explorers)
    - [Blockchain Databases and Analyzers](#ton-blockchain-databases-and-analyzers)
    - [Other](#ton-other)
    - [API](#ton-api)
- [SMARTCONTRACTS](#smartcontracts)
- [METAVERSE](#metaverse)
- [NFT](#nft)
    - [NFT Databases and Analyzers](#nft-databases-and-analyzers)
    - [API](#nft-api)
- [IPFS](#ipfs)
- [METAVERSE](#metaverse)
- [DEFI](#defi)
- [DORK](#dork)
- [NOTABLE ACCOUNT TO FOLLOW](#notable-accounts-to-follow)
- [TOOLS](#tools)
- [RESOURCES, REFERENCES, READING](#resources-references-reading)
- [LEAKS?](#notable-breach-and-leaks-related-to-web3)

### CRYPTO-OPSEC Methodologies and Info 
| Info / Tool | Description |
| --- | --- |
[OfficerCIA Guide](https://github.com/OffcierCia/Crypto-OpSec-SelfGuard-RoadMap) | Collection and discussion about the best DeFi,Blockchain and crypto-related OpSec researches

## <img src="https://cryptologos.cc/logos/bitcoin-btc-logo.png" alt="btc" style="width:25px;" width="25" height="25" /> Bitcoin - BTC

### BTC Address Regex
| Address regex | Description |
| --- | --- |
| `1[a-z0-9A-Z]{25,33}` | Legacy addresses |
| `3[a-z0-9A-Z]{25,33}` | P2SH address |
| `bc1[a-z0-9A-Z]{23,42}` | Segwit addresses |
| `bc1p[a-z0-9A-Z]{23,42}` | Taproot addresses |

### BTC Blockchain explorers
| Link | Description |
| --- | --- |
| [3xpl.com](https://3xpl.com/bitcoin) | Fastest ad-free universal block explorer |
| [Blockchain.com](https://www.blockchain.com/explorer/assets/btc) | One of the first and robust explorer, it permits to explor Bitcoin, Ethreum, Bitcoin Cash , other Assets and also NFT  |
| [Blockchair](https://blockchair.com/bitcoin) | An explorer that supports differents cryptovalutes, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block |
| [Crystalblockchain](https://explorer.crystalblockchain.com/) | The public explorer helps to search for adresses, transactions, it also display a comprensive detail about ad address. |
| [Tokenview](https://tokenview.io/) | Another blockcahin explorer, it supports different tokens and cryptocurrencies, BTC, ETH, XMR ... Search info by addresses and or trnsactions  |
| [Graphsense](https://graphsense.github.io/)| GraphSense is a cryptoasset analytics platform emphasizing full data sovereignty, algorithmic transparency, and scalability.    |
| [Coincodex](https://coincodex.com/crypto/bitcoin/historical-data/) | Hystorical price of Bitcoin |
| [Awebanalysis](https://awebanalysis.com/en/bitcoin-address-validate/) | Validate Bitcoin format |
| [WalletExplorer](https://www.walletexplorer.com/) | A service which try to retrieve the wallet related to an address [#BacarefullwhatyouOSINTWith](https://www.theblock.co/linked/118223/chainalysis-used-an-ip-scraping-block-explorer-to-aid-law-enforcement-leaked-docs-say)  |
| [Breadcrumbs.app](https://www.breadcrumbs.app/) | An investigation tool that help to visualize address relation, it's very helpful and it contains information about sanzioned address and assets. It supports BTC, ETH and any ERC20 Token |
| [TRM](https://www.trmlabs.com/) | TRM Tranasction Monitor and TRM Forensics are two tools that help in dept analysis on Blockchain transactions  | 
| [Lampyre](https://lampyre.io/) | Like Maltego it supports BTC investigations and correlations. [#BacarefullwhatyouOSINTWith](https://keyfindings.blog/2020/03/23/be-careful-what-you-osint-with/)  |
| [Bitquery.io](https://www.bitquery.io/) | Full explorer which support, addresses analysis, smartcontracts and assets explorer |
| [Ciphertrace](https://www.ciphertrace.com/) | Inspect/Armada - Cryptocurrency Risk and Fraud Controls for Financial Institutions/Cryptocurrency Risk and Fraud Controls for Financial Institutions |
| [Coinfirm](https://www.coinfirm.com/) | industry-leading blockchain analytics, investigations and AML solutions are trusted to best analyse and manage risk.|
| [Whalealert](https://whale-alert.io/alerts) | An alerting system, it's helpful to get alerts when wallets with a big amount of funds are making transactions |
| [BTCparser](https://btcparser.com/) | A project to get information about differents kind of wallets, it monitors old wallets or wallets related to the Satoshi era |
| [Bitref](https://bitref.com) | A simple, address explorer. It display amount of Bitcoin held on given addresses |


### BTC Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [CryptoBlacklist](https://www.cryptoblacklist.io/en/bitcoin-blacklist/) | An addresses blacklist, it contains simple reports about the type of activities the address is related to |
| [Bitcoinwho'swho](https://www.bitcoinwhoswho.com/) | An address lookup service to indify report related to a malicious BTC addresses. |
| [Bitcoinabuse](https://www.bitcoinabuse.com/) | Tracking bitcoin addresses used by ransomware, blackmailers, fraudsters, etc. |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA |
| [Scamsearch](https://www.scamsearch.io/) | It's a global scam database. Search by Profile Picture, Email, Username, Pseudo Name, Phone Number, crypto address or website. |
| [Scamalert](https://scam-alert.io/) | It offers a search engine for scam and crypto-address related frauds  |
| [Cryptoscamdb](https://cryptoscamdb.org/scams) | A scam database which contains information about sites scam and related address  |
| [Ransomwhere](https://ransomwhe.re/) | Bitcoin address used in ransomware activities, the databse is in raw format and it's integrated in chainabuese service |
| [Know Your Coin Privacy](https://kycp.org/) | Try to guess relation from BTC adddress using this techiques  Boltzmann analysis, Entity analysis, Address reuse, Input/output merges |
| [SPLcenter Addresslist](https://www.splcenter.org/cryptocurrency-report) | A spreadsheet containing information about address used by extremists and far right communities |
| [Bad Bitcoin](https://badbitcoin.org/) | A database containing info and details about Bitcoin Fraud since 2014 |
| [Vivigle](https://vivigle.com/) | A global cryptoRatings and Analytics Platform |

### BTC API
| Req | Description |  
| --- | --- |  
| `https://3xpl.com/bitcoin/address/xxx` | Request for the status of the address using 3xpl API |
| `https://blockchair.com/bitcoin/address/xxx` | Request for the status of the address using Blockchair API |  
| `https://blockchair.com/bitcoin-cash/transaction/xxx` | Request for the detail of a give Transaction |  
| `https://www.bitcoinabuse.com/reports/` | Looking for any entry related to a given address on the Bitcoinabuse database |  
| `http://codacoin.com/api/public.php?request=validate&address=xxx` | An api for get a validation of a given BTC address |  
| `https://blockchain.info/q/24hrprice` | Retrieving the price of the last 24h |  
| `https://blockchain.info/q/getreceivedbyaddress/xxx` | Retrieving the amount received on a given BTC address  |  
| `ttps://blockchain.info/q/getsentbyaddress/xxx` | Retrieving information of what was sent by a given address |  
| `https://blockchain.info/q/addressbalance/xxx` | Retrieving the balance for a given address |  
| `https://chain.api.btc.com/v3/address/xxx` | Retrieving information about a given address |  
| `https://blockchain.info/q/addressfirstseen/xxx` | It retrieve the first seen date of a given address |  

### BTC Other
| Link | Description |
| --- | --- |
| [CriminalIP](https://www.criminalip.io/login?h=/asset/search?query=%22Bitcoin%22%20port:%208333) | It'a a infrstructure scanner. It scans ip and services, there is a section related to miner services exposed online |
| [Intelx.io](https://intelx.io/) | It indexes nformation retrieved from both closed and open source. It also indexs IP, email, BTC addresses and other kind of assets |
| [Antianalysis](https://antinalysis.org/example) | Service is maintened and hosted by activist, it support machine learning to analyze information about an address and its related transactions |
| [Antianalysis (DARK)](http://pdcdvggsz5vhzbtxqn2rh27qovzga4pnrygya4ossewu64dqh2tvhsyd.onion/about) | Service is maintened and hosted by activist, it support machine learning to analyze information about an address and its related transactions | 
| [Cryptocurrencyalerting](https://cryptocurrencyalerting.com/wallet-watch.html) | Getting alerts about transaction related to a given address |
| [Localbitcoin](https://localbitcoins.com/) | Useful to check nicknames and details that could be related to Bitcoins adopters
| [Aware Online](https://www.aware-online.com/en/osint-tools/cryptocurrency-search-tool/)| Different tools to conduct Osint investigation on given BTC addresses |
| [GraphSense Maltego Transform](https://github.com/INTERPOL-Innovation-Centre/GraphSense-Maltego-transform) | A Maltego transform which leverage the power of GraphSense for Crypto investigations |
| [Mempool Space](https://mempool.space/it/) | A graphical dashboard to analyze history fo block congestion, fee, lighting networks and mining activities 

## <img src="https://cryptologos.cc/logos/ethereum-eth-logo.png" alt="btc" style="width:25px;" width="25" height="25"  /> Ethereum - ETH

### ETH Address Regex
| Address regex | Description |
| --- | --- |
| `0x[0-9A-Fa-f]{40}` |  All Ethereum addresses have a length of 40 hexadecimal characters and begin with “0x” |

### ETH Blockchain explorers
| Link | Description |
| --- | --- |
| [3xpl.com](https://3xpl.com/ethereum) | Fastest ad-free universal block explorer. |
| [Blockchain.com](https://www.blockchain.com/explorer/assets/eth) | One of the first and robust explorer, it permits to explor Bitcoin, Ethreum, Bitcoin Cash , other assets and also NFT  |
| [Etherscan](https://etherscan.io/) | The most reliable and complete explorer for Ethereum ecosystem. It help to search Adressess, token , nft, smartcontracts and other also ens domains |
| [Blockchair](https://blockchair.com/bitcoin) | An explorer that supports differents cryptovalutes, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block |
| [Tokenview](https://tokenview.io/) | Another blockcahin explorer, it supports different tokens and cryptocurrencies, BTC, ETH, XMR ... Search info by addresses and or trnsactions  |
| [Blockscout](https://blockscout.com/eth/mainnet/) | It covers all about ethereum, from transactions and block information, token values to sidechains and private chains 
| [Ethective](https://ethtective.com/)| could be a great help for our forum investigators because has a very interesting way to visualize Ethereum network, that makes exploring transfers much more interactive.    |
| [Graphsense](https://graphsense.github.io/)| GraphSense is a cryptoasset analytics platform emphasizing full data sovereignty, algorithmic transparency, and scalability.    |
| [BitQuery](https://explorer.bitquery.io/bitcoin?theme=dark) | A Blockchain explorer which supports different kind of assetts. It supports BTC, ETH, DOGE, ADA etc |
| [Ethplorer](https://ethplorer.io/) | Track address portfolios for any Ethereum address with comprehensive balance charts and transactions; |
| [ENS Domains](https://app.ens.domains/) | An ens domain explore, mainly used to purchase that kind of assets, it also help to find end domains and related information |
| [Breadcrumbs.app](https://www.breadcrumbs.app/) | An investigation tool that help to visualize address relation, it's very helpful and it contains information about sanzioned address and assets. It supports BTC, ETH and any ERC20 Token |
| [Arkhamintelligence](https://platform.arkhamintelligence.com) | A tool that permits network mapping on DEFI and altcoin related entities, currently in closed BETA
| [Watchers.pro](https://watchers.pro) | [Warning!!! Create a sock wallet, it needs a Metamask extension to access it] A tool that provides a dashboard for clustering and inspecting DEFI and altcoin related entities 

### ETH Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [CryptoBlacklist](https://www.cryptoblacklist.io/en/ethereum-blacklist/) | An addresses blacklist, it contains simple reports about the type of activities the address is related to. |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA |
| [Scamsearch](https://www.scamsearch.io/) | It's a global scam database. Search by Profile Picture, Email, Username, Pseudo Name, Phone Number, crypto address or website. |
| [Cryptoscamdb](https://cryptoscamdb.org/scams) | A scam database which contains information about sites scam and related address  |
| [Cryptoscam](https://cryptscam.com/) | Another database containing information about scammers, it supports Email/Address search
| [SPLcenter Addresslist](https://www.splcenter.org/cryptocurrency-report) | A spreadsheet containing information about address used by extremists and far right communities |
| [Vivigle](https://vivigle.com/) | A global cryptoRatings and Analytics Platform |
| [Walletlabels](https://www.walletlabels.xyz/) | Search engine based on a collection of more than 7.5M ETH labeled addresses | 

### ETH Other
| Link | Description |
| --- | --- |
| [Chat Blockscan](https://chat.blockscan.com/index) | A chat based on Ethereum blockchain, useful to reach an ens domain or address owner |
| [CriminalIP](https://www.criminalip.io/login?h=/asset/search?query=%22Ethereum%22%20port:%208545)|  It'a a infrstructure scanner. It scans ip and services, there is a section related to miner services exposed online |
| [Naddison36](https://github.com/naddison36/tx2uml) | Ethereum transaction to UML sequence diagram generator |
| [Cryptocurrencyalerting](https://cryptocurrencyalerting.com/wallet-watch.html) | Getting alerts about transaction related to a given address |
| [Aware Online](https://www.aware-online.com/en/osint-tools/cryptocurrency-search-tool/)| Different tools to conduct Osint investigation on given ETH addresses |
| [GraphSense Maltego Transform](https://github.com/INTERPOL-Innovation-Centre/GraphSense-Maltego-transform) | A Maltego transform which leverage the power of GraphSense for Crypto investigations |
| [Etherscan Transforms for Maltego](https://www.maltego.com/transform-hub/etherscan/) | The official Etherscan transform for Maltego

## <img src="https://cryptologos.cc/logos/monero-xmr-logo.png" alt="monero" style="width:25px;" width="25" height="25" /> [](#monero)MONERO - XMR

### XMR Address Regex
| Address regex | Description |
| --- | --- |
| <code>(4&#124;8)[1-9A-Za-z]{94}</code> | A raw Monero address is a set of 95 characters starting with a '4' or an '8 |

### XMR Blockchain Explorers
| Link | Description |
| --- | --- |
| [Blockchair](https://blockchair.com/monero) | Help to inspect transactiosn and related hashes. |

### XMR Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Antianalysis](https://antinalysis.org/example) | Service is maintened and hosted by activist, it support machine learning to analyze information about an address and its related transactions |
| [Antianalysis (DARK)](http://pdcdvggsz5vhzbtxqn2rh27qovzga4pnrygya4ossewu64dqh2tvhsyd.onion/about) | Service is maintened and hosted by activist, it support machine learning to analyze information about an address and its related transactions | 

## <img src="https://cryptologos.cc/logos/cardano-ada-logo.png" alt="cardano" style="width:25px;" width="25" height="25" /> [](#cardano)CARDANO - ADA

### ADA Address Regex
| Address regex | Description |
| --- | --- |
| `Ae2[1-9A-HJ-NP-Za-km-z]+` | Legacy address ( Byron ) - Icarus-style |
| `DdzFF[1-9A-HJ-NP-Za-km-z]+` | Legacy address ( Byron ) - Daedalus-style |
| `addr1[a-z0-9]+` | Shelley address  |
| `stake1[a-z0-9]+`  | Shelley address used in stacking pool |

### ADA Blockchain explorers
| Link | Description |
| --- | --- |
| [Blockchain.com](https://www.blockchain.com/explorer/assets/ada) | One of the first and robust explorer, it permits to explor Bitcoin, Ethreum, Bitcoin Cash , other Assets and also NFT |
| [Cardano explorer](https://explorer.cardano.org/en)| The official scanner for Cardano transactions, it help to analyze addresses, transactions for each epoch |
| [Blockchair](https://blockchair.com/cardano) | An explorer that supports differents cryptovalutes, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block.  |
| [Adastat](https://adastat.net/)| An explorer related to the whole Cardano ecosystem, it can inspect Addresses, Block, Trnsactions Epoch   |
| [Adapool](https://adapools.org/) | An Stacking pool explorer, it helps to browse stacking pool and the currently related activities  |
| [BitQuery](https://www.bitquery.io/) | Full explorer which support, addresses analysis, smartcontracts and assets explorer |

### ADA Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA |

## <img src="https://cryptologos.cc/logos/solana-sol-logo.png" alt="solana" style="width:25px;" width="25" height="25" /> [](#solana)SOLANA - SOL

### SOL Address Regex
| Address regex | Description |
| --- | --- |
| `[1-9A-HJ-NP-Za-km-z]{32,44}` | A Solana address's length varies from 32 to 44 characters. |

### SOL Blockchain explorers
| Link | Description |
| --- | --- |
| [Solana Explorer](https://explorer.solana.com/) | The official scanner for Solana transactions, it help to analyze addresses, transactions, tokens    |
| [Blockchair](https://blockchair.com/solana) |  An explorer that supports differents cryptovalutes, Bitcoin, Ethereum, Dogecoin, the search permits to query address, transaction and embedded text inside block.   |
| [Solscan.io](https://solscan.io/) | A Solana scanner which support Address, transaction, token and NFT 

### SOL Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Chainabuse](https://www.chainabuse.com/) | Report a cryptocurrency hack or scam across multiple blockchains and search addresses and domains to see if they are connected to any fraudulent activity. It supports BTC, ETH, SOL and ADA |

## <img src="https://cryptologos.cc/logos/thumbs/toncoin.png" alt="ton" style="width:25px;" width="25" height="25" /> [](#toncoin) TONCOIN - TON

### TON Address Regex
| Address regex | Description |
| --- | --- |
| `0:[a-z0-9]{64}` | The raw address, it is an hexadecimal format  
| `[a-zA-Z0-9\-\_]{48}` | Friendly name, based on a custom hash algorithm, ref: crc16 custom #TODO investigate
| `\w\s\w\s\w` | It also supports generated nickname like `Graceful Tan Takin` <_<

### TON Blockchain explorers
| Link | Description |
| --- | --- |
| [3xpl.com](https://3xpl.com/ton) | Fastest ad-free universal block explorer |
| [Tonscan](https://tonscan.org/)  | An address lookup service, it helps to find details about a given address |
| [Ton.sh](https://ton.sh) | An address lookup service, it helps to find details about a given address, it support API   |
| [Tonmoon](https://tonmoon.org/explorer/)| Help to inspect an address, it support canonical address and nickname also |
| [Youton](https://youton.org/)| Another Address explorer   |
| [Toncoin](https://explorer.toncoin.org/) | An more technical esplorer, it helps to query the TON network using different keyfields, workchain ,shard and so on |
| [TonAPI](https://tonapi.io/swagger-ui) | Is a platfor and API useful for inspect TON address and any related assets, it supports Number and also NFT  |
| [Ton.page](https://ton.page/) | Another Explorer, fast and easy to use
| [Ton.cx](https://ton.cx/) | A raw and in depht analysis tool for TON transactions
| [GetGems](https://getgems.io/top-collections/) | A marketplace for NFTs for TON network assets |


### TON Blockchain Databases and Analyzers
| Link | Description |
| --- | --- |
| [Ton known addresses](https://catchain.github.io/tonscan/src/addrbook.json) | List of known TON Addresses


### TON OTHER
| Link | Description |
| --- | --- |
| [Tonwine](https://ton.wine/) | An interactive way to pay with TON |
| [Fragment](https://fragment.com/numbers) | Is a marketplace/ auction used to purchase number or nickname usable on the Telegram platform `https://fragment.com/username/[username]` |
| [Ton place](https://ton.place/) | A platform for monetize from content and fanbase, dork `site:ton.place [content]` |
| [Tonex](https://tonex.app/) | A social netowrk directly integrated on TON network
| [TONwhale](https://tonwhales.com/it/explorer/top) | A list of top 1000 accounts 
| [TONmeterbot](https://tonometerbot.com/) | A service used to make scores about users. The score is generated on Balance/NFTnum basis. 
| [ATOP](https://github.com/aaarghhh/a_TON_of_privacy) | A tool for make investigation on TON NFTs like Telegram fake numbers, Telegram nickname, and TON domain.

### TON API
| Link | Description |
| --- | --- |
| Get bulk info about some addresses | ```curl -X 'GET' 'https://tonapi.io/v1/account/getBulkInfo?addresses=0%3Ada6b1b6663a0e4d18cc8574ccd9db5296e367dd9324706f3bbd9eb1cd2caf0bf%2C0%3Ada6b1b6663a0e4d18cc8574ccd9db5296e367dd9324706f3bbd9eb1cd2caf0bf' -H 'accept: application/json'``` |
| Search for a ton domain | ```curl -X 'GET' 'https://tonapi.io/v1/dns/domains/search?domain=wallet.ton' -H 'accept: application/json'``` | 
| Search all Telegram number currently not on sale (limit 10000) | ```curl -X 'GET' 'https://tonapi.io/v1/nft/searchItems?collection=0%3A0e41dc1dc3c9067ed24248580e12b3359818d83dee0304fabcf80845eafafdb2&include_on_sale=false&limit=10000&offset=0' -H 'accept: application/json```
| Get a backresolve of a domain | ```curl -X 'GET' 'https://tonapi.io/v1/dns/backresolve?account=0%3ABA60BFBD527C0CD2D70C6396630C50A498AF015B987ADAAD1D4A9E287F604536' -H 'accept: application/json'``` |
| Get current bids for a domain | ```curl -X 'GET' 'https://tonapi.io/v1/auction/getBids?domain=wallet.ton' -H 'accept: application/json'``` | 

## SMARTCONTRACTS
| Tool | Description |
| --- | --- |
|[PALKEO](https://oko.palkeo.com/) | An Ethereum explorer focused on smart contracts |
|[Ethereum Signature Database](https://www.4byte.directory/) | A database containing the bytes related to functions used in Database  |
|[Grep.app](https://grep.app/search?q=solidity) | Search for smartcontract source code. It could be useful for search for nft or contract sourcecode |
|[EIS3](https://github.com/salaheldinaz/EIS3) | A ENS domain (.eth domain) analyzer 


## NFT
| Tool | Description |
| --- | --- |
| [Opensea](https://opensea.io/) | The first and more relevant NFTmarketplace, it also supports ENS name, accounts could be explorer using this pattern: https://opensea.io/[nickname]  |
| [Binance NFT](https://www.binance.com/en/nft/) | NFT marketplace directly managed by Binance |
| [Rarible](https://rarible.com/) | Another NFT marketplace, it supports ETH, SOL, Thezos and Polygon |
| [Coinbase](https://nft.coinbase.com/) | NFT marketplace directly managed by Coinbase |
| [Crypto.com](https://crypto.com/nft)|  NFT marketplace directly managed by Crypto.com |
| [NFT Calendar](https://nftcalendar.io/) | A Calendar for NFT project, it doesn't require any author validation |
| [Luckyblock](https://nft.luckyblock.com/explore/collections) | NFT explorer for NFT minted on the BNB network |
| [Nftsearch](https://nftsearch.site/) | A reverse search for finding NFT, it supports images, address and so on |
| [NFTfinder](https://www.nyckel.com/nft-finder/) | A reverse search for finding NFT, it supports images, address and so on | 
| [Compass](https://compass.art/pulse) | An explorer which help to understand statistics about NFTs |
| [Context.app](https://context.app) | An NFT explorer mainly related to owners, it should synk Twitter followers to their address or ENS name |
| [NFT Analyst Starter Pack](https://github.com/a16z/nft-analyst-starter-pack) | USing alchemy API key, it can generate CSV extracts for all token transfers, historical sales, and each underlying item's metadata |
| [Nftfreeviewer](https://www.freenftviewer.io/) | An NFTs epxlorer that supports ETH and Polygon netowrk |
| [Tonnft](https://explorer.tonnft.tools/) | A marketplce and explorer for TON nft |
| [GetGems](https://getgems.io/top-collections/) | Another marketplace for NFTs for TON network assets |
| [Disintar](https://beta.disintar.io/) | A marketplace for NFTs based on TON netowrk, there is also a collection related to Telegram names |
| [NFTGO.io](https://nftgo.io/) | Discover, analyze, and trade NFTs faster and smarter than anyone else, aided by in-depth analytics and intelligent toolkits. |
| [NFT scan](https://www.nftscan.com/) | An nft explorer which supports different blockchain like Ethereum, Binance, Polygon, Solana and others


### NFT Databases and Analyzers
| Link | Description |
| --- | --- |
| [Scamsniffer](https://explorer.scamsniffer.io/?sort=30DayVolume) | A full solution to track NFT scammer, it also supports a Browser extension and a Discord bot |


### NFT API
| Tool | Description | API CALL |
| --- | --- | --- |
| [Alchemy API](https://www.alchemy.com/nft-api) | Help to navigate ETH and other chain data via API | `import { Alchemy } from "alchemy-sdk";Alchemy().nft.getNftsForOwner("0xshah.eth").then(console.log);` |


## IPFS
| Tool | Description |
| --- | --- |
| `ipfs dht findprovs <hash-of-file>` | returns IDs of all nodes having the file |
| `ipfs dht findpeer <nodeID>` | returns the list of node addresses (IP v4 and v6, TCP and UDP) |
| [IPFS scanner](https://github.com/cryptodashie/ipfs/tree/fda709851b21d9ef82eb246da6f96667f14f3ae8)| IPFS scanning can identify new hosted content or expose information leaks similar to Amazon S3 buckets.  | 
| [IPFS browser](https://ipfsbrowser.com/) | Search, view, access, and download IPFS files quickly and easily right in your web browser from any device! |

## METAVERSE
| LINK | Description |
| --- | --- |
| [Spatial](https://www.spatial.io) | An example of Metaverse, it contains different spaces where people can connect with. `https://www.spatial.io/@[USERNAME]`   |


## DORK
| Dork | Description |
| --- | --- |
| `[ADDRESS] -block` | Identify information related to the address but not indexed by common search engines  |
| `site:[url of interest] [ADDRESS]` | help to find information about an address on a target url of interest |
| `(antminer) AND protocols.raw: “80/http” AND 80.http.get.title: “401”` | (Shodan) dork for antminer |
| `ETH - Total Speed` | (Shodan) Claymore Miner Software |


## NOTABLE ACCOUNT TO FOLLOW
| Breach | Description |
| --- | --- |
| [CIA_Officer](https://twitter.com/officer_cia) | Independent Security Researcher • Not the CIA • OpSec & Privacy Guru • On-Chain & OSINT Sleuth
| [Rugpullfinder-(Inactive)](https://twitter.com/rugpullfinder) | The NFT community's premier source of information |
| [ZachXBT](https://twitter.com/zachxbt) | On-chain sleuth. Rug pull survivor turned 2D detective 


## TOOLS
| Breach | Description |
| --- | --- |
| [Obsidian templates Cryptocurrencies](https://github.com/theNerdInTheHighCastle/obsidian-osint-templates/blob/main/--%20templates/crypto-address.md) | An Obisidian template for Cryptocurrencies investigations  |
| [Obsidian templates NFT](https://github.com/theNerdInTheHighCastle/obsidian-osint-templates/blob/main/--%20templates/NFT.md)| An Obisidian template for NFT investigations  |
| [Eth Explorers Extension](https://github.com/apoorvlathey/eth-explorers-extension) | Browser extension to open Ethereum addresses & transaction hash from any page on popular explorers + dashboards |
| [Maltego](https://www.maltego.com/)| Maltego directly support BTC and ETH address entities. It is a tool used for OSINT and Forensic investigations   |
| [Tatum Blockchain Explorer (Maltego Transofrm)](https://www.maltego.com/) | Tatum is a blockchain development platform that supports over 40 blockchain protocols and 2000 + digital assets.   |
| [Opensanctions (Maltego Transofrm)](https://www.maltego.com/) | A transform for Maltego, it queries sanctioned address from opensaction database |
| [Cyphertrace Explorer (Maltego Transform)](https://www.maltego.com/) | The Cypertrace' transform for Maltego 
| [EMER name (Maltego Transform)](https://github.com/Tomasuh/Maltego_Transform_Blockchain_DNS/tree/63e6fb152a75893103ec038b9974db937ba21baa) | Useful transform to resolve EMER domain names |


## RESOURCES, REFERENCES, READING
| Resource | Description |  
| --- | --- |  
| [Cia Operator Start.me](https://cia.start.me/p/dlaxD0/ciaofficerv2) | The start.me of CIA operators, and infinite source of news and interesting tools  |
| [Crypto Mindmaps](https://cryptoengineer.notion.site/cryptoengineer/9f1668632aa04a0a83a311a86e799254?v=f7c5c49231f44b91a44021411fa27e28) | Useful mindmaps related to  crypto and WEB3 |
| [Tornadocash after censorship](https://hackmd.io/@gozzy/tornado-cash-post-censorship) | A guide to bypass Tornadocash censorship  
| [WEB3 is going great](https://web3isgoinggreat.com/) | Daily news about what's going wrong on Crypto and WEB3
| [The Nerd in the high castle](https://thenerdinthehighcastle.wordpress.com) | OSINT and FORENSICS tutorial and articles


## NOTABLE BREACH AND LEAKS RELATED TO WEB3
| Breach | Description |
| --- | --- |
| Bitcointalk |2015, database of one of the first community directly involved in BTC growth |
| BTC-E | Account balances, Email addresses, IP addresses, Passwords, Usernames, Website activity  |
| BTC-Alpha | Email addresses, IP addresses, Passwords, Usernames |
| Globalcrypto.exchange | Hacked by CoomingProject ransomware operators >__> |
| Ledger | A list of info related to Ledger user, it was leaked in 2022 and cointains user details |
| Coinmarketcap| A list of email scraped from Coinmarketecap platform |
| Coinmama | Email addresses, Passwords, Usernames |
| Bitcoin Lixter | Combolit |
| Bit2Visitor | Combolist |
| BitcoinRush.io | Combolist |
| BitLeak.net | Combolist |
| Atlas Quantum | Account balances, Email addresses, Names, Phone numbers |
| BitsCircle | Combolist (Credential stuffing?) |
| BitLeak.net | Combolist (Credential stuffing?) |
| GateHub | Email addresses, Encrypted keys, Mnemonic phrases, Passwords of the online wallet service |
| BitsCircle.com | Combolist (Credential stuffing?) |
| BTC4Free.com | Combolist (Credential stuffing?) |
| BTC60.net | Combolist (Credential stuffing?) |
| ButterflyLab.com | Combolist (Credential stuffing?) |
| Feathercoin.com | Combolist (Credential stuffing?) |
| MtGox.com | Combolist (Credential stuffing?) |
| ShoppingBitcoins.com | Combolist (Credential stuffing?) |
| Dagpay.io | Mail,password,IP,id of the SCAM project Dagocoin |
| Paybito | Hitted by Lockbit ransomware gang >__> |
| BitRewards | bitrewards.com 2020 full database |
| BitMain | Bitmain database 2018 |
| Cointracker | 2022 compromised Email and partial telephone number |
| Gemini | 2022 email phone number |
| Blockachain.com | 307K emails |

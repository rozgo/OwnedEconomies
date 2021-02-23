# OwnedEconomies Exchange - Ultra-light Paper

## Abstract
Many communities, games and apps need to own their economies in order to provide a safe, engaging, trustworthy, fair and value-preserving user experience. We present a blockchain architecture for developing custom exchanges that host privately owned economies, tokenomics and liquidity.

## Goals
- Blockchain-based platform with the simplicity of traditional consumer products
- Capture tangible and intangible value while preserving sovereignty
- Ability to model high frequency economics and governance

## Use Cases
- Affiliation and loyalty programs
- Curation, rewards and royalty systems
- User-generated content markets
- Delivery, mobility and logistics markets
- Gig economies
- Massive-multiplayer games
- IoT fleets and robot swarms

## Core Architecture
Our architecture builds upon [Substrate](https://substrate.dev/), a modular framework that enables the creation of purpose-built blockchains by composing custom or pre-built components. Substrate leverages strongly-typed systems for modeling the application domain.
 
The private chain needs only to serve the community, thus, there is no need for gas, or network fees. Difference governance models can incentivize proper resource utilizations. Consensus is based on [Proof of Authority](https://academy.binance.com/en/articles/proof-of-authority-explained).

## Asset Types
- Fungible assets
- Non-fungible assets
- Proof of ownership assets (certificates, permissions, memberships)
- Live assets - mutating assets that react to triggers and/or change over time (melt, evaporate, die, combine)
- Bundle - an algebraic asset, a structured asset that’s formed by composing other assets.
 
Simple tokens are insufficient for modeling the economy.
 
## Exchange Rates
Exchange rates are based on asset bundle pairs; not just simple asset pairs. This improves upon traditional exchanges that fail to capture restrictions, requirements, externality costs, combo offers, proof of ownership, etc; as part of a transaction. A reference implementation can be found [here](https://github.com/Simbotic/smartcontract-multiagent/blob/master/src/account.rs).
 
This sophisticated exchange system can model:
- Crafting systems
- Skill/leveling trees
- Dense rewards for reinforcement learning
- Business workflows
- Government transactions
- KYC regulations
- and many, many more
 
## Simulation
Unlike many other blockchain technologies, our stack is constantly simulating the economy, triggering spatial, timed and flow events. Not only is it bot-friendly, but automation is encouraged. Ideal for research, persistent games, automated market makers (AMMs), etc. The end goal is to optimize for a continuos, interactive and provably fair economics simulation.
 
## Liquidity
The main liquidity outlet is an [Ethereum Bridge](https://github.com/Snowfork/polkadot-ethereum). A light Ethereum client embedded in our custom blockchain to bridge with MainNet. Users can lock their assets on Ethereum using smart contracts and bridge liquidity to our private economy. It does not involve any third parties, and assets are locked by the chain. Hence, trustless.
 
## Minimum Viable Product
The amazing folks from [Polkadot](https://polkadot.network/) and [Polkadex](https://www.polkadex.trade/) provide a treasure trove of blockchain components, UI frameworks and APIs for rapid development. As components mature and/or diverge we can transition to more ground-up developed components.

- [API](https://github.com/polkadot-js/api) - Promise and RxJS APIs around any Substrate-based chain RPC calls. It is dynamically generated based on what the Substrate runtime provides in terms of metadata.
- [App](https://github.com/polkadot-js/apps) - Basic Substrate UI for interacting with a node. This is the main user-facing application, allowing access to all features available on Substrate chains.
- [Blockchain Components](https://substrate.dev/docs/en/knowledgebase/runtime/frame) - Substrate is composed of several smaller components for defining types, storage items, and functions.

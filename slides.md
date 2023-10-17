# Building in Public

## The EIP process

---

## Show of hands if you:
---


## Show of hands if you:

- have ever opened an issue on a public Github repo
---

## Show of hands if you:

- have ever opened an issue on a public Github repo (other than your own)
---


## Show of hands if you:

- have ever opened an issue on a public Github repo (other than your own)
- have ever contributed a PR to an open source project
---


## Show of hands if you:

- have ever opened an issue on a public Github repo (other than your own)
- have ever contributed a PR to an open source project
- have ever participated in any sort of discussion on a programming language spec update/change
---

## You
____

Have built in public.  Well done.
---

## Building in Public
___
**Not original to me**
- Building software in public is at least as old as the internet
- The Linux kernel, Python, most open source software, are all built in public
- Ethereum is almost entirely built in public
---


# Ethereum Improvement Proposal (EIP)
___
- A proposed change in the Ethereum specification or a new standard entirely
- Can be as simple as a minor tweak to signature verification (EIP150)
- A new token standard (EIP/ERC20)
- A complete overhaul of how gas fees are computed (EIP1559)
---

## Who does EIPs?
___
---

## Ethereum Foundation researchers
___
![Vitalk Buterin](/vitalik.jpg)
Like this guy.
---

## People from the community
___
- Client teams - Geth, Nethermind, Besu, etc.
- Applications - Uniswap, Ethers.js, etc.
---

## Anyone with a Github profile
___
Like this totally...
---

## Anyone with a Github profile
___
Like this totally...anonymous...
---

## Anyone with a Github profile
___
Like this totally...anonymous...pineapple.
![Protolambda](/proto.png)
---

## The anatomy of an EIP
___
---

Summary/Abstract - the TLDR
___
**EIP-1559**

"A transaction pricing mechanism that includes fixed-per-block network fee that is burned and dynamically expands/contracts block sizes to deal with transient congestion."
---

Motivation - How we got here
___
**EIP-4337**

"See also https://ethereum-magicians.org/t/implementing-account-abstraction-as-part-of-eth1-x/4020 and the links therein for historical work and motivation, and EIP-2938 for a consensus layer proposal for implementing the same goal.

This proposal takes a different approach, avoiding any adjustments to the consensus layer. It seeks to achieve the following goals:

Achieve the key goal of account abstraction: allow users to use smart contract wallets containing arbitrary verification logic instead of EOAs as their primary account. Completely remove any need at all for users to also have EOAs (as status quo SC wallets and EIP-3074 both..."
---

Specification - What we are proposing in this change, usually in great detail with code examples
___
**EIP-3855**

"The instruction PUSH0 is introduced at 0x5f. It has no immediate data, pops no items from the stack, and places a single item with the value 0 onto the stack. The cost of this instruction is 2 gas (aka base)."
---

Rationale - Why we are proposing this change
___
**EIP-3675** (i.e. the Merge)

"The changes specified in this EIP target a minimal requisite set of consensus and client software modifications to safely replace the existing proof-of-work consensus algorithm with the new proof-of-stake consensus represented by the already in-production beacon chain.

This EIP was designed to minimize the complexity of hot-swapping the live consensus of the Ethereum network..."
---

Various other details
___
- Backwards Compatibility

EIP-2098 -- "The Compact Representation does not collide with canonical signature as it uses 2 parameters (r, yParityAndS) and is 64 bytes long while canonical signatures involve 3 separate parameters (r, s, yParity) and are 65 bytes long."
- Security Considerations
- Test cases
- Appendices
- Etc.
---

# The lifecyle of an EIP
___
![EIP lifecycle](/EIP-process-update.jpg)
---

## Idea
_____
- Ethereum research forums (ethresear.ch, Ethereum Magicians)
- Discussion in Ethereum R&D Discord server
---

## Draft
____
- A PR opened on the https://github.com/ethereum/EIPs repository
- A presentation to the community
  - AllCoreDevs community calls
  - EIP proposals in research forums
- Author works with EIP editors to ensure draft is formatted properly
---

## Review
____
- PR merged into EIP repository
- EIP revisions in conjunction with community feedback
- Further discussion on ACDC (not the band, but almost as good) or other working groups
- EIP implemented in Ethereum client software (or other code as necessary)
- EIP functionality rigorously tested (devnets/testnet deployments)
- "Considered for inclusion" - the final stage
---

## Final
____
- EIP is considered a complete/finalized specification
- Scheduled for inclusion in a hardfork (i.e. upgrade) to Ethereum
---

# EIP-4844 - a case study
____

---

## Idea
____
- Make data availability cheaper for rollups who post data on Ethereum mainnet
- "Shard Blob Transactions" - an Ethereum transaction with a bunch of arbitrary data attached to it
- "Protodanksharding" - the name given to the specific approach used in 4844 to provide data availability 
- Started in winter 2022 with a post from Vitalik Buterin (Ethereum co-founder) on Ethereum Magicians and some early prototypes built at EthDenver by protolambda and others
---
## Draft
____
- [PR](https://github.com/ethereum/EIPs/pull/4844) opened in Feb, 2022
---

## Review
____
- PR merged on March 2, 2022
- Development began in earnest by client teams in summer 2022
- First devnets launched fall 2022
- "CFI"-d for Cancun hardfork in winter 2023
- We're now on devnet-9
---

## Final
____
- **Soon**...
---

# Links
____

- [EIPs](https://eips.ethereum.org/)
- [EIP Repo](https://github.com/ethereum/EIPs)


![QR](/qr.png)
---

___
**Ask me anything, really!**
---
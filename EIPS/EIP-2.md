## Preamble

    EIP: 2
    Title: Decentralized governance
    Author: Eric Muyser <eric@muyser.com>
    Type: Standard Track
    Category: Core
    Status: Draft
    Created: 2018-01-26

## Simple Summary

A standard for decentralized governance of a blockchain ecosystem.

## Abstract

Smart contracts on a decentralized blockchain allowing for robust management of a decentralized organization. A standardized protocol for representatives to propose and action changes, and users in tehe ecosystem to elect those representatives.

## Specification

### Republic

The Republic is made up of elected representatives ("Delegates"), who are responsible for the management and decision making of significant matters. These Delegates are voted into power by token holders ("Citizens"). When dealing with matters that drastically affect the Republic and the Citizens, Delegates can hold polls to gauge their constituents. For example, voting to overhaul architecture or do a rollback. In most situations, Delegates will be able to resolve issues amongst themselves, in an open forum. Delegates will follow a set of rules and guidelines in making decisions ("Constitution"). By creating the structure and constitution that will dictate the management of the Hyperbridge Technology ecosystem, the development and deployment of technology is not driven by a singular person or group; rather, the collective will of token-holders is to be reflected by their elected representatives. 

Hyperbridge Technology will hold all delegatory positions initially. Within a one to two year timeframe these seats will be transferred to elected industry leaders. When all 11 seats are occupied, the Token Holders will gain primary voting rights over the delegation members of the Republic. Delegates will initially be chosen by the founders of the Republic, Hyperbridge Technology. Delegates will be chosen based on their leadership and the contributions made with in their respective industry. After the republic has been formed and all Delegates have been placed, elections will be held biyearly (every 2 years), giving Citizens a chance to rotate Delegates.

Voting power will be a 40/60 split between the Republic and Citizens. The Republic will have 40% voting power (666,666,666 voting shares), and Citizens will have 60% voting power (1,000,000,000 voting shares). A single Republic Token (REF) will be worth 1 voting share. Republic seat holders ("Delegates") are required to abide by rules of governing the ecosystem ("Constitution"). The Constitution outlining the specific standards of this model is in development and will be made available to the public before Delegates are appointed. Delegates can be voted in and out by the majority. Like any democratic organization, the will of the community is expected to be upheld by the appointed delegates. If delegates act against the will of the community, not upholding the will of the people, a sufficient argument must be provided so as to protect their seat. We believe 11 Delegates is small enough to provide both decentralization and balance, while being small enough to coordinate changes to the system. A 40/60 stakeholder balance provides the community with enough power so that if they need to use it they can, but not so much so that it becomes over-distributed and unfocused. Most of the time, the Republic can operate without need for community voting. In rare circumstances, the community may need to vote for major changes or seat holders.

### Republic Token

Republic will issue an ERC20 standard token[1] on the Ethereum network, Republic Token (REF). There will be a limited supply of 1,000,000,000 REF tokens.

Basic functionality available with a Republic token:
* Appointment of Republic delegates through industry elections
* Delegated governance over any Republic-compatible smart contracts
* Issue resolution through token holder votes

All precautions will be taken to secure the limited unchanging supply of REF. We will take all precautions to secure the tokens, however in the unfortunate event of a hack, we have prepared a plan. If a significantly large sum of REF has been stolen, minted, or burned, Republic will reissue the tokens on a new smart contract to represent the authentic token state of a point in history before the hack took place. Republic will then need to work with integrations to migrate to the new contract. In the future, it’s possible Republic will support REF on more blockchains than Ethereum. If this is to happen, as part of the Constitution, Republic will not inflate the number of tokens. A smart contract would be created for new blockchains, with 0 REF, and users will be given a way to convert the REF they own on Ethereum. At any one time, there will only ever be 1,000,000,000 tokens across all blockchains.

### Senate

The Senate is a body of representatives elected by token holders ("Citizens") and the Senate itself based on the voting power hereto described. The Senate has power over the chosen ecosystem by way of access rights and built directly into the smart contracts. The Senate also has power of municipal districts (often dApps) and their local representatives ("Congress").

### Congress

If so chosen, a dApp can form a body of representatives for the management of their smart contracts. Within their contracts, they integrate management by way of the Republic Token, which gives them local management of their contracts, but with the security of a higher level body of representatives, the Senate. The Senate has power over the Congress, and can vote to replace or remove the Congress if found to be needed. The reasoning behind the Congress is for scalability of leadership and development decision making and progress.

### Primary Election

Every 6 months, a Primary election will be held. This election is composed of 11 Industry elections, where Citizens can nominate themselves as leaders in each category. The Primary election contract can only be interacted with by the Republic contract.


### Industry Election

Every Primary election will have a set number of Industry elections. Initially there will be 11. Industry elections can only be started and managed by the Primary election contract.

### Citizens (Token Holders)

Token Holders will be known as Citizens within the Republic.

## Rationale

The need for decentralized governance is to capitalize on the true benefit of offering a blockchain-based ecosystem. We need an ecosystem that is not subjected to the full force of a centralized entity, as such an entity can be shut down or corrupted (potentially through new leadership or owners). Initially all seats in the Republic will belong to Hyperbridge Technology Inc. No way was seen to avoid this and innovate at the same time. Hyperbridge will actively seek out industry leaders with a strong desire to actively participate in the management of the ecosystem.

## References

1. hyperbridge/republic-protocol PR #4, https://github.com/hyperbridge/republic-protocol/pull/4

## Copyright

Copyright and related rights waived via [CC0](https://creativecommons.org/publicdomain/zero/1.0/).
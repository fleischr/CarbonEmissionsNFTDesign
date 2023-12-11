# EmissisionsNFTDesign
Emissions NFT Design Docs

## Organization Smart Contract
Organizations deploy a smart contract with a standard interface and mint NFTs from it to represent scope 1, 2, and 3 emissions

The whitelist to mint NFTs from the contract will belong to members of the organizations

By default, the minting contract can accommodate an unlimited number of mints

Ability to mint will be constrained by the block timestamp

## Emissions NFTS

A from-date timestamp and to-date timestamp will be required at mininum for every mint

The emissions NFT may be indicative of one or more business activities or transactions

Level of granularity in emissions reporting/tokenization is up to the organization to decide. Generally, its assumed organizations will increase granularity over time.

Emissions NFTs may have hierarchical relations to another for either cross-organizational scope 3 emissions

## Alternate representations

Every emissions NFT have alternate verifiable representations as decentralized id (DID) documents and zero knowledge proofs

The emissions NFT shall provide functions that offer on-chain verifiability for the DID documents and zero knowledge proofs

Alternate representations may offer additional data characteristics not represented in the NFT itself

Alternate representations can be persisted permanently on blockchains (ex: IPFS, transactions hashes) or other data sources

## Emissions measurement and verification

Emissions as CO2 equivalent in metric tonnes

1 milligram is to be the smallest possible unit of precision emissions measurement (e.g. 0.000000001). Generally measurements with precision within 1 kilogram are still considered excellent.

3rd parties can add quality rating signatures, referencing specific alternate representations


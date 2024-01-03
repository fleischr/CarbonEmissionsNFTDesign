# EmissisionsNFTDesign
Emissions NFT Design Docs

## Organization Smart Contract
Organizations deploy a smart contract with a standard interface and mint NFTs from it to represent scope 1, 2, and 3 emissions

The whitelist to mint NFTs from the contract will belong to members of the organizations

By default, the minting contract can accommodate an unlimited number of mints

Ability to mint will be constrained by the block timestamp

## Emissions NFTS

Emissions NFTs are minted as token-bound accounts with [ERC-6551](https://eips.ethereum.org/EIPS/eip-6551)

A from-date timestamp and to-date timestamp will be required at mininum for every mint

The emissions NFT may be indicative of one or more business activities or transactions. It is primarily time bound above all other criteria

Level of granularity in emissions reporting/tokenization is up to the organization to decide. Generally, its assumed organizations will increase granularity over time.

Emissions NFTs may have hierarchical relations to another for either cross-organizational scope 3 emissions

Emissions NFT as a token bound account can hold balances of other tokens - used to represent the present cost/profit or the financial liability/asset of the given set of carbon emissions

## Alternate representations

Every emissions NFT have alternate verifiable representations as verifiable credential (VC) documents and zero knowledge proofs

The emissions NFT shall provide functions that offer on-chain verifiability for the VC documents and zero knowledge proofs

Alternate representations may offer additional data characteristics not represented in the NFT itself

Alternate representations can be persisted permanently on blockchains (ex: IPFS, transactions hashes) or other data sources - but this is not required

## Emissions measurement and verification

Emissions are measured as CO2 equivalent in metric tonnes

1 milligram is to be the smallest possible unit of precision emissions measurement (e.g. 0.000000001). Generally measurements with precision within 1 kilogram are still considered excellent.

3rd parties can add quality rating signatures, referencing specific alternate representations. The smart contract can automatically verify the signatures of the identities -while the zero knowledge proofs can offer verifiability of the "off-chain" data itself.

## Common, but optional extensions
Precision -- indicates the preferred level of mathematical precision of measure meant
Nabla -- indicates the assumed level of emissions for the given time period and business activity
Delta -- documents expected an actual change in emissions
Parents -- Publically verified high level emissions NFTS (e.g. related scope 1 emissions to scope 3 emissions)
Children -- Publically verified high level emissions NFTS (e.g. related scope 3 emissions to scope 1 emissions)


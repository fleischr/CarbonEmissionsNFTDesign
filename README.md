# CarbonEmissionsNFTDesign
Carbon Emissions NFT Design Docs

## Organization Smart Contract
Organizations deploy a smart contract with a standard interface and mint NFTs from it to represent scope 1, 2, and 3 emissions

The whitelist to mint NFTs from the contract will belong to members of the organizations

By default, the minting contract can accommodate an unlimited number of mints - but the ability to mint will be constrained by the block timestamp

## Emissions NFTS

Emissions NFTs ideally are minted as token-bound accounts with [ERC-6551](https://eips.ethereum.org/EIPS/eip-6551) that are further anchored to a DID registry that supercede the organization. That is the ultimate design goal - however prototype development may yet use typical ERC721 or storage smart contract templates as a starter.

A from-date timestamp and to-date timestamp will be required at mininum for every mint

The emissions NFT may be indicative of one or more business activities or transactions. It is primarily time bound above all other criteria

Level of granularity in emissions reporting/tokenization is up to the organization to decide. Generally, its assumed organizations will increase granularity over time.

Emissions NFTs may have hierarchical relations to another for either cross-organizational scope 3 emissions

Emissions NFT as a token bound account can hold balances of other tokens - used to represent the present cost/profit or the financial liability/asset of the given set of carbon emissions

## Emissions NFT Alternate representations

Every emissions NFT have alternate verifiable representations as verifiable credential (VC) documents and zero knowledge proofs

The emissions NFT shall provide functions that offer on-chain verifiability for the VC documents and zero knowledge proofs

Alternate representations may offer additional data characteristics not represented in the NFT itself that are otherwise likely to be found in private data storage (ex: SAP)

Alternate representations can be persisted permanently on blockchains (ex: IPFS, transactions hashes) or other data sources - but this is not required

Overall - alternate representations are meant for emissions data conform to the Axiomatic Data Assets specification

## Emissions measurement and verification

Emissions are measured as CO2 equivalent in metric tonnes

1 milligram is to be the smallest possible unit of precision emissions measurement (e.g. 0.000000001). Generally measurements with precision within 1 kilogram are still considered excellent.

3rd parties can add quality rating signatures, referencing specific alternate representations (e.g. a verfied credential, IPFS data store, ZKP). The smart contract is meant support a maximum level of verifiability within given privacy constraints

## Carbon Emissions Data Verifier workflow

An independent 3rd party verifier may access an organization's carbon emissions data for auditing per the GHG Protocol standard

Using a DID - the carbon auditor may produce and digitally sign their attestations of the quality of the organizations emissions mitigation effors and the data thereof. These attestations can be maintained at least in part by the NFT smart contract - with additional supplements through alternate representations (Verified Credentials, zero knowledge proofs) and other conventional data stores (private databases, cloud storage)

## Advanced capabilities
The usage of token bound accounts is meant to support multiple token types which may compose the GHG summary overall

## Additional References
See [Additional References](./REFERENCES.md)

## Demo implementations
App level : GHG Template App on SAP BTP

Smart contract level : VeChain Microgrant

## Contributors
Ryan Fleischmann

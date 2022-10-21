<!--
Guiding Principles:

Changelogs are for humans, not machines.
There should be an entry for every single version.
The same types of changes should be grouped.
Versions and sections should be linkable.
The latest version comes first.
The release date of each version is displayed.
Mention whether you follow Semantic Versioning.

Usage:

Change log entries are to be added to the Unreleased section under the
appropriate stanza (see below). Each entry should ideally include a tag and
the Github issue reference in the following format:

* (<tag>) \#<issue-number> message

The issue numbers will later be link-ified during the release process so you do
not have to worry about including a link manually, but you can if you wish.

Types of changes (Stanzas):

"Features" for new features.
"Improvements" for changes in existing functionality.
"Deprecated" for soon-to-be removed features.
"Bug Fixes" for any bug fixes.
"Client Breaking" for breaking Protobuf, gRPC and REST routes used by end-users.
"CLI Breaking" for breaking CLI commands.
"API Breaking" for breaking exported APIs used by developers building on SDK.
"State Machine Breaking" for any changes that result in a different AppState given same genesisState and txList.
Ref: https://keepachangelog.com/en/1.0.0/
-->

# Changelog


## Current - 2022-10-21

### Bug Fixes

* [\#2](https://github.com/sei-protocol/sei-cosmos/pull/2) Fix GRPC bug

### Improvements

* [\#1](https://github.com/sei-protocol/sei-cosmos/pull/1) Integrate Cosmos with sei-tendermint and ABCI++
* [\#14](https://github.com/sei-protocol/sei-cosmos/pull/14) Integrate Cosmos with Tendermint tracing
* (x/auth/vesting) [\#11652](https://github.com/cosmos/cosmos-sdk/pull/11652) Add util functions for `Period(s)`


### Features
* [\#17](https://github.com/sei-protocol/sei-cosmos/pull/17) Support SR25519 algorithm for client transaction signing
* [\#23](https://github.com/sei-protocol/sei-cosmos/pull/23) Add priority to CheckTx based on gas fees
* (x/accesscontrol)[\#24](https://github.com/sei-protocol/sei-cosmos/pull/24) Add AccessControl module
* [\#27](https://github.com/sei-protocol/sei-cosmos/pull/27) Add tx channels for parallel DeliverTx signaling 
* (x/accesscontrol)[\#30](https://github.com/sei-protocol/sei-cosmos/pull/30) Add resource hierarchy helper to build resource dependencies
* (x/accesscontrol)[\#33](https://github.com/sei-protocol/sei-cosmos/pull/33) Add gov proposal handler for x/accesscontrol
* (x/accesscontrol)[\#41](https://github.com/sei-protocol/sei-cosmos/pull/41) Add ante dependency decorator to define dependencies
* [\#58](https://github.com/sei-protocol/sei-cosmos/pull/58) Lazy deposits all module accounts during EndBlock for parallel DeliverTx
* (x/accesscontrol)[\#59](https://github.com/sei-protocol/sei-cosmos/pull/59) Add gov proposal type for wasm dependency mapping updates
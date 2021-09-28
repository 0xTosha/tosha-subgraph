# Tosha Subgraph

TheGraph exposes a GraphQL endpoint to query the events and entities within the Binance Smart Chain and 0xtosha ecosystem.

Currently, there are multiple subgraphs, but additional subgraphs can be added to this repo:

1. **[Blocks](https://thegraph.com/legacy-explorer/subgraph/0xtosha/blocks)**: Tracks all blocks on Binance Smart Chain.

2. **[Exchange](https://0xtosha.medium.com/0xtosha-info-relaunch-in-partnership-with-150-000-bounty-winner-streamingfast-f7892559d388)**: Tracks all 0xtosha Exchange data with price, volume, liquidity, ...

3. **[Farm Auctions](https://thegraph.com/legacy-explorer/subgraph/0xtosha/farm-auctions)**: Tracks all 0xtosha Farm Auctions with auctions and bids.

4. **[Lottery](https://thegraph.com/legacy-explorer/subgraph/0xtosha/lottery)**: Tracks all 0xtosha Lottery with rounds, draws and tickets.

5. **[NFT Market (v1)](https://thegraph.com/legacy-explorer/subgraph/0xtosha/nft-market)**: Tracks all 0xtosha NFT Market for ERC-721.

6. **[Pairs](https://thegraph.com/legacy-explorer/subgraph/0xtosha/pairs)**: Tracks all 0xtosha Pairs and Tokens.

7. **[Pancake Squad](https://thegraph.com/legacy-explorer/subgraph/0xtosha/pancake-squad)**: Tracks all Pancake Squad metrics with Owners, Tokens (including metadata), and Transactions.

8. **[Prediction (v1)](https://thegraph.com/legacy-explorer/subgraph/0xtosha/prediction)**: Tracks all 0xtosha Prediction (v1) with market, rounds, and bets.

9. **[Prediction (v2)](https://thegraph.com/legacy-explorer/subgraph/0xtosha/prediction-v2)**: Tracks all 0xtosha Prediction (v2) with market, rounds, and bets.

10. **[Profile](https://thegraph.com/legacy-explorer/subgraph/0xtosha/profile)**: Tracks all 0xtosha Profile with teams, users, points and campaigns.

11. **[SmartChef](https://thegraph.com/legacy-explorer/subgraph/0xtosha/smartchef)**: Tracks all 0xtosha SmartChef (a.k.a. Syrup Pools) with tokens and rewards.

12. **[Timelock](https://thegraph.com/legacy-explorer/subgraph/0xtosha/timelock)**: Tracks all 0xtosha Timelock queued, executed, and cancelled transactions.

13. **[Trading Competition (v1)](https://thegraph.com/legacy-explorer/subgraph/0xtosha/trading-competition-v1)**: Tracks all metrics for the Easter Battle (April 07—14, 2021).

## v1

To access subgraphs related to 0xtosha v1 ecosystem ([article](https://0xtosha.medium.com/the-great-migration-vote-4093cb3edf23)), use [`v1`](https://github.com/0xtosha/pancake-subgraph/tree/v1) branch.

## To setup and deploy

For any of the subgraph: `blocks` as `[subgraph]`

1. Run the `cd subgraphs/[subgraph]` command to move to the subgraph directory.

2. Run the `yarn codegen` command to prepare the TypeScript sources for the GraphQL (generated/*).

3. Run the `yarn build` command to build the subgraph, and check compilation errors before deploying.

4. Run `graph auth --product hosted-service '<ACCESS_TOKEN>'`

5. Deploy via `yarn deploy`.

# 📊 LigerSwap Pairs Subgraph 🐯

TheGraph exposes a GraphQL endpoint to query the events and entities within the Binance Smart Chain and LigerSwap ecosystem.

Currently, there are multiple subgraphs, but additional subgraphs can be added to this repository, following the current architecture.

## Subgraphs

**[Pairs](https://thegraph.com/hosted-service/subgraph/xliger/pairs)**: Tracks all LigerSwap Pairs and Tokens.

## Dependencies

- [Graph CLI](https://github.com/graphprotocol/graph-cli)
    - Required to generate and build local GraphQL dependencies.

```shell
yarn global add @graphprotocol/graph-cli
```

## Deployment

For any of the subgraph: `pairs` as `[subgraph]`

1. Run the `cd subgraphs/pairs` command to move to the subgraph directory.

2. Run the `yarn codegen` command to prepare the TypeScript sources for the GraphQL (generated/*).

3. Run the `yarn build` command to build the subgraph, and check compilation errors before deploying.

4. Run `yarn graph auth --product hosted-service '<ACCESS_TOKEN>'`

5. Deploy via `yarn deploy`.



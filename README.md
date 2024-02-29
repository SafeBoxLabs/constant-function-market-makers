# constant-function-market-makers

The repository hosts a collection of bots that simulate various market-making strategies currently utilized on blockchain platforms through the use of constant function market maker (CFMM) curves. It's important to note that certain behaviors inherent to on-chain market making cannot be fully replicated due to the unique properties of smart contracts, which only change state in response to user interactions. This document will highlight a few such behaviors, including:

- FIFO (First In, First Out) Ordering
- Real-time Limit Order Rebalancing
- Incorporation of External Market Data

The bots are characterized by several attributes that influence their operational mechanisms, specifically in the context of limit order management. These attributes include:

- The strategy for placing limit orders, which could be a predetermined rate or an initialization parameter
- The approach to modifying existing limit orders, categorized as either static (unchanged) or dynamic (subject to change)
- The method of fulfilling limit orders, which could involve using the bot's own inventory or sourcing liquidity from an external decentralized exchange (DEX)
- The interrelationship of their limit orders, which might follow a specific pattern such as a constant, a CFMM curve, a Logarithmic Market Scoring Rule (LMSR), a Balancer Weighted Curve, etc.

# What is a "Sandwich Attack"? How to Check if You’ve Been Targeted?

A sandwich attack is a common on-chain malicious trading strategy, typically involving high-frequency trading bots (often called "MEV bots"). These bots quickly buy and sell tokens to exploit price differences, sometimes engaging in front-running or manipulating gas fees to execute trades ahead of regular users, profiting from price changes.

If you notice the following signs, you may have been targeted by a sandwich attack:

1. **Significant Price Difference**: The actual price of your trade is much different from the price a second ago.
2. **Synchronized Trades**: Before and after your transaction, there is a buy order and a sell order from the same address.
3. **Bot Labeling**: Your trading address is flagged as a bot on platforms like DEXTools.
4. **Typical Trade Size**: Bot trades usually range between $6,000 and $9,000.
5. **Your Trade Type**: You placed a buy order.

If your trade doesn't match these patterns, it’s likely that someone else executed a trade before yours, causing the price to spike. To protect yourself from such attacks, you can enable **MEV Protection** in PumpX, which helps mitigate this risk.

# Why Is My Limit Order Executing at a Different Price?

On decentralized exchanges (DEX), order execution differs from centralized exchanges (CEX), which can result in discrepancies between your limit order price and the actual transaction price.

* **Order Book Model on CEX**: On centralized exchanges, trading is managed through an order book system, where prices are determined by active buy and sell orders. When you place a limit order (e.g., buying at $0.001), the transaction will be executed at that price as long as there is a matching sell order. The price remains fixed, and your order will be executed exactly at your set price without slippage.
* **Automated Market Maker (AMM) Model on DEX**: Most DEXs, like Uniswap and Sushiswap, use an AMM model, where prices are determined by liquidity pools. These pools use a formula (x \* y = k), with prices based on the ratio of tokens in the pool, which dynamically changes with each trade. As a result, the price of your limit order depends on the current ratio of tokens in the pool, not the price you set. For example, if you place an order to buy at $0.001, the actual price may change when the transaction is executed, especially if the trade size is large and affects the pool balance. This could result in your final price being $0.0015 instead.

1.  Slippage

    * **What is Slippage?** Slippage refers to the difference between the expected price of a trade and the price at which it’s actually executed. This is common on DEXs, particularly with larger trades.
    * **Why Does Slippage Occur?** Slippage happens because AMM models adjust prices based on liquidity pool changes. If the pool has low liquidity, your trade can have a larger impact on the price, resulting in more slippage.
    * **Managing Slippage**: Most DEXs let you set slippage. If your slippage is too low, the trade may fail or execute at a significantly different price. Typically, slippage can be set between 0.1% and 50%. Higher slippage increases the likelihood of your trade going through, but may result in a worse price.


2.  Liquidity Issues

    * **Liquidity Depth**: The depth of liquidity in a pool is essential for price stability. If the pool has sufficient liquidity, your trade will not cause large price fluctuations, and the actual price will closely match your order. However, in shallow pools, larger trades can push the price away from your limit.
    * **Liquidity Pools**: In AMM systems, prices are determined by the ratio of two tokens in the liquidity pool. As you execute a trade, the ratio and price change accordingly. This is why a limit order set at $0.001 may end up executing at a higher price, like $0.0015.


3.  Gas Fees and Transaction Priority

    * **Impact of Gas Fees**: On-chain transactions require gas fees, which can influence the speed and priority of your trade. If you set a low gas fee, your transaction may be delayed. In volatile market conditions, this delay can cause the price to change before the transaction is processed.
    * **Block Confirmation Time**: The time it takes for a transaction to be confirmed depends on network congestion and the gas fee you choose. During this confirmation period, prices may fluctuate, especially in low liquidity pools or volatile markets.


4.  Price Impact in AMM Models

    * **Large Transactions and Price Impact**: In AMM systems, large trades can significantly affect the token ratio in the pool, causing the price to deviate further from your original order. For example, placing a large buy order at $0.001 could shift the token ratio, leading to the trade executing at a price lower than expected.
    * **Price Curve Impact**: In AMM systems, prices don’t change in a straight line. Small trades cause slight price movements, but larger trades lead to more significant shifts. This can result in a greater difference between your limit order price and the actual executed price.



**How to Minimize Price Differences:**

1. Choose liquidity pools with deeper liquidity.
2. Set a reasonable slippage (though this may increase the risk of trade failure).
3. Split large orders into smaller trades.
4. Use higher gas fees to speed up transaction processing.

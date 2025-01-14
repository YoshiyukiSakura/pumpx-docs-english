# Why Are Gas Fees So High?

**What is Gas?**\
Gas fees are the charges paid to validators and the blockchain network for each transaction. Every transaction requires gas, and these fees are not collected by PumpX.

**Why Are Gas Fees Higher for Token Purchases Than for Transfers?**\
Gas fees are tied to the complexity of the operation, the computational resources required, and the storage needs on the blockchain. Purchasing tokens involves complex contract logic and frequent state updates, while transferring tokens is simply moving assets from one address to another—a much simpler process that requires fewer computational resources.\
**Note:** Some special tokens have particularly complex smart contracts, leading to abnormally high gas fees for each transaction. This is why the gas fees for buying tokens are typically higher than for transfers.

**What are Priority Fees and Speed Modes?**\
Priority fees (often referred to as "tips") were introduced with Ethereum’s EIP-1559 upgrade. This mechanism allows users to pay an additional fee on top of the base gas fee in order to speed up transaction processing. Transactions with higher fees are typically prioritized, so users can adjust the fee to control how quickly their transactions are confirmed. You can select normal, fast, or priority modes in the transaction settings to adjust both the fee and speed.\
Keep in mind that lower fees may result in slower processing times and even transaction failure. During times of high demand, such as token launches or market surges, lower priority fees could lead to failed transactions.

**Are Gas Fees Fixed?**\
No, gas prices fluctuate dynamically depending on network congestion. When the network is busy, gas fees rise to incentivize validators to prioritize transactions; during quieter periods, gas fees decrease. The gas price displayed on the transaction page reflects the price from the previous second and can change rapidly, so it should be considered an estimate.

**Why Do Gas Fees Fluctuate So Much?**\
Gas fees on Ethereum can vary significantly due to several factors, including supply and demand on the network, market bidding dynamics, transaction complexity, major market events, and the strategies used by validators to bundle transactions. As transaction demand increases, gas fees can quickly spike, especially during congested periods. Historically, gas fees have exceeded 1000 Gwei, and in extreme cases, they have briefly surpassed 2000 Gwei. Typically, the gas price for a token transaction is around 30 Gwei, with fees ranging from $20 to $50.

**Why Am I Charged Gas Fees Even if My Transaction Fails?**\
Gas fees represent the computational cost on the blockchain to execute a transaction or contract and are mandatory fees. PumpX does not charge these fees. Once your transaction details are packed by PumpX onto the blockchain, the blockchain processes the computation and determines if the transaction cannot be completed, leading to a failure. As a result, gas fees are non-refundable, even if the transaction fails.

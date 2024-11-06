# FAQs

#### [V1 Users](faqs.md#v1-users-1)

#### [Yield Market](faqs.md#yield-market-1)

#### [Dual Yield for Apes](faqs.md#dual-yield-for-apes-1)

#### [Cross-margin](faqs.md#cross-margin-1)

### V1 Users

Q: Can I use my ERC20 tokens as collateral in BendDAO V2?

A: Yes! BendDAO V2 allows you to use both NFTs and ERC20 tokens as collateral.



Q: I am a BendDAO V1 borrower. Can I earn yield as well?

A: Unfortunately, no. The NFT cannot be re-collateralized. You’ll need to fully repay your V1 loan before joining V2 for NFT-backed staking.\


Q: Can I still delegate my NFT when using V2?

A: Yes! Both V1 and V2 fully support delegation via delegate.cash V2.



Q: How is the value of my NFT calculated?

A: The NFT value is determined using a TWAP (Time-Weighted Average Price) provided by the BendDAO’s NFT oracle.



Q: How is the value of ERC20 tokens calculated?

A: ERC20 token values are calculated using Chainlink’s Oracle solution, integrated seamlessly with BendDAO.



Q: What is the main difference between BendDAO V1 and V2?

A: BendDAO V1 primarily focuses on NFT lending, while V2 expands to support both NFTs and ERC20 tokens, offering more yield strategies and capital efficiency.

### Yield Market

Q: What are the benefits of staking my NFTs on V2?

A: Yield! By staking your NFTs, you’ll earn yield from restaking and re-depositing your borrowed assets, boosting your overall returns.\


Q: Why is there no liquidation risk?

A: V2 is designed to eliminate liquidation risk by automatically unstaking assets before a liquidation event could occur. This ensures your NFTs are never subject to forced liquidation.\


Q: How to make sure that I can always make profit if I keep paying the interests?

A:  Based on historical APR data from third-party staking protocols over the past few months, we’ll keep the rate curve volatility below the average.

For example, if Lido’s average is 3%, we’ll set the staking lending curve between 1% and 3%, with 3% marking the utilization rate approaching its limit.



Q: Can I still delegate my NFT when staking?

A: Yes, BendDAO supports delegate.cash, so you can still delegate your NFTs while staking on V2.



Q: Is there a waiting period for unstaking? How long will it take for my NFT to return to my wallet?

A: There’s no waiting period. Once the transaction is completed, your NFT will be unstaked and returned to your wallet immediately.



Q: What happens if the NFT floor price drops significantly? I don’t want to face liquidation.

A: If the floor price hits a critical threshold, the smart contract will automatically unstake your NFT, ensuring no liquidation will occur.



Q: How is the yield from restaking calculated?

A: Yields are calculated based on the protocols where your assets are restaked, taking into account base rewards, additional incentives, and compound interest.



Q: Can I earn dual yields on V2?

A: Yes! If you own BAYC or MAYC, you can earn both ApeCoin and additional returns through V2’s yield strategies.\


### Dual Yield for Apes

Q: I’m staking through the ApeCoin official site. Can I earn dual yields?

A: Yes, you can still earn dual yields by staking your BAYC or MAYC NFTs through BendDAO V2, receiving both ApeCoin rewards and additional yield from the V2 yield market.



Q: Can I borrow other assets while staking my NFT?&#x20;

A: Sorry, no. Because you borrowed amount are used to restaking/redeposting to third-party protocols, like Lido, EtherFi.



Q: Is there a cap on how much I can earn from dual yields?

A: The yield depends on the third-party protocol and the utilization of the liquidity of V2.&#x20;



Q: Can I stake multiple NFTs at once?

A: Yes, the batch staking is supported.

\
Cross-margin

### Cross-margin&#x20;

Q:  How to know my loan health factor?

A:  In V2, the health factor is calculated in the account base which means if you have enough value depositing, even your collateral value drops a lot, you account can still be safe. For more details, refer to the [liquidation page](concepts/liquidation.md). \


Q:  How to avoid my NFTs to be liquidated?

A:  Since in V2, cross-margin is supported. Users can increase the account health factor by depositing more ERC20 tokens and NFTs.&#x20;

\


\


\






\

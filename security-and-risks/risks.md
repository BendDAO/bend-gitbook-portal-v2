# Risks

{% hint style="info" %}
By using BendDAO, you assume the risks associated.

The following section provides an overview of different types of risks you should be aware of when using our protocol.

This overview is not exhaustive and may not cover all potential risks to which you might be exposed.
{% endhint %}

BendDAO is committed to use industry-leading security practices. Yet, there are still a number of risks associated with the use of V2 protocol that users must be aware of.

## Smart contract risk

There is an inherent risk that the protocol could contain a smart contract vulnerability or bug.

Several security measures are employed to mitigate this risk:

* The code is a simple and public-sourced code base that avoids complexities.
* The code has been audited by external security company, in addition to a competitive security review.
* There's ongoing bug bounty programs on Immunefi.

More details about V2's security and security reviews can be found in the dedicated section.

## Oracle risk

Every V2's lending pool is connected to oracle, established at pool creation. The oracle is integrated with well-know third-party protocol such as Chainlink. It is important to understand that no oracle is immune to price manipulation, which can lead to liquidations or even bad debt. However, some oracles will be more resistant and resilient than others.

When assessing the reliability of an oracle, consider factors such as safety and liveness, particularly if the oracle is centralised. Also, take into account the settings and processes pertaining to the definition and frequency of price updates.

## Counterparty risk

Before entering a lending pool, it's crucial to conduct thorough due diligence on the loan asset and the collateral asset to understand who holds power over them. Factors to consider include centralisation, as a centralised governance could blacklist a specific user, resulting in a loss of funds. The distribution of the asset is also important, as a high concentration can cause extreme price fluctuations.

## Liquidation risk

### Liquidation risk (for borrowers)

Each asset in V2's lending pool is linked to an Loan-to-Value (LTV) and Liquidation Threshold (LTH). If the debt of your position exceeds this LTH, you will face liquidation. When borrowing on V2, carefully select the lending pool asset and diligently manage the health of your position.

### Bad debt risk (for lenders)

There could be circumstances in which the collateral's value for a position drops below the borrowed amount before liquidators can close the position. In such cases, the borrower holding this position has no incentive to repay the debt. BendDAO should use treasury funds to cover bad debts through governance, but it still may result in an immediate loss for the lenders.

### Liquidity risk (for lenders)

Liquidity refers to the access to supplied assets. A lack of liquidity can prevent suppliers from withdrawing their assets for a certain period of time. Liquidity issues are tackled through the interest rate model. Before providing liquidity, it's essential to understand the pool's interest rate model. This understanding will help you estimate the level of liquidity you can expect in that market.

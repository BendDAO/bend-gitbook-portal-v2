# Yield Market

We can build yield markets based on the [leverage lending](leverage-lending.md) in V2 protocol.

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Yield Market</p></figcaption></figure>

### NFT-backed Staking – Without Liquidation Risk

NFT-backed staking taps into incentive structures within Restaking and DeFi protocols, allowing borrowed assets to be staked and earn rewards from reputable platforms. Since the borrowed assets are exclusively used within selected protocols, the risk of liquidation is eliminated.

How It Works:

1. Stake NFT on V2
2. Borrow and Restake/Re-supply: Borrow the asset and restaking/re-supply same asset, creating a recursive loop that amplifies the initial stake and boosts the overall returns.
3. Incentive Capture: With each loop, you accumulate base rewards and potential incentives, driving up the total APY and maximizing yield.

This strategy increases returns without exposing users to the liquidation risks typical of leveraged positions.

### Dual Yields for Apes

BAYC and MAYC holders can benefit from dual yields, allowing Apes to earn both ApeCoin and additional returns through V2’s yield strategies. This approach maximizes the rewards from holding Apes, optimizing overall returns without liquidation risk.

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### Liquidation

There's **NO liquidation** for the staking in yield markets, and the heath-factor in the staking is only used for unstake forcefully if the HF below certain value (e.g. default is 1.05).

The definition for Health Factor:

SUM(All Collaterals Value) / SUM(All Debts Value).

Collateral Value = NFT Floor Price \* Collateral Factor + Yield Token Amount \* Yield Token Price.

Debt Value = Debt Token Amount with interest \* Debt Token Price.

For example, Using BAYC in Lido Staking:

**At the beginning**:

BAYC Floor Price = 20 ETH;

Borrow Amount = 20 ETH \* 5 = 100 ETH, staked in the Lido Protocol;

**After the staking in some days**:

stETH Price = 0.9997 ETH;

Yield Amount = 101 stETH, with some staking yield;

Collateral Value = 20 ETH \* 0.9 + 101 \* 0.9997 ETH = 118.9697 ETH;

Debt Value = 100.5 ETH, with some borrow interest;

Health Factor = 118.9697 / 100.5 = 1.1837781094527364;

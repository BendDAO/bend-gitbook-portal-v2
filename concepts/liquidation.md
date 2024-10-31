# Liquidation

{% hint style="info" %}
This contents is only for the lending in V2 protocol. There's no liquidation for the staking in yield markets.
{% endhint %}

The V2 Protocol utilises a scored 'health factor' for debts. Liquidation will be triggered if the debt's health factor is below 1.

## Meaning of Health Factor <a href="#meaning-of-health-factor" id="meaning-of-health-factor"></a>

The definition for Health Factor:

SUM(All Collaterals Value) / SUM(All Debts Value).

The risk level of the health factor:

* 0.0 < HF < 1.0: <mark style="color:red;">Dangerous</mark>, borrower maybe lose collateral if the debt is not repaid timely.
* 1.0 <= HF <= 1.5: <mark style="color:orange;">Risky</mark>, borrower should repay partly the debt timely.
* 1.5 < HF < 2.0: <mark style="color:yellow;">Careful</mark>, borrower should pay attention and monitor the debt timely.
* 2.0 <= HF: <mark style="color:green;">Safe</mark>, borrower no need to worry and keep the debt last.

## Cross Margin Lending

When an account becomes unhealthy, meaning its Loan-To-Value (LTV) on a given market exceeds the market’s Liquidation Threshold (LT), the account’s position can be liquidated. Anyone can perform this liquidation by repaying the account’s debt in exchange for the equivalent amount in the market collateral asset, along with an incentive (Bonus).

To avoid being liquidated, borrowers can track their LTV in real-time and either repay their loan, partially or entirely, either add more collateral to their position.

Liquidations on V2 protocol are quite simple: liquidators can liquidate up to 100% of the account’s debt and receive the corresponding collateral value, plus the relative incentive.

No fee is taken by the V2 protocol at this level. The entire Liquidation Bonus goes to the liquidator.

## Isolate Margin Lending

When the 'health factor' of an NFT loan is below 1, anyone can trigger a liquidation in terms of an NFT Auction. The liquidator is called Bidder on BendDAO. The bidder will pay back all of the debt and receive the collateralised NFT in return. The borrower can redeem his NFT to exit auction by repaying some loan debts (50% in default).

## Staking in Yield Market

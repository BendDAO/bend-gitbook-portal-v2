# Interest Rate Models

V2 is an Interest Rate Model (IRM) agnostic protocol, meaning it can support any interest rate model for its lending pool assets. In V2, the interest borrowers pay in a given asset is defined by the IRM chosen at asset listing among a governance-approved set.

## Rationale

Bend’s interest rate model is calibrated to manage liquidity risk and optimize utilization. The borrow interest rates come from the Utilization Rate $$U$$.

$$U$$ is an indicator of the availability of capital in the pool. The interest rate model is used to manage liquidity risk through user incentivizes to support liquidity:

* When capital is available: lower interest rates to encourage loans.
* When capital is scarce: higher interest rates encourage repayments for the loans and additional deposits.

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption><p>Interest Curve Example</p></figcaption></figure>

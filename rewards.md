---
description: >-
  OpenWorld Rewards provide benefits for long-term users of the protocol, these
  rewards come in the form of Escrowed OPEN and Multiplier Points.
---

# Rewards

## Compounding vs Claiming

There are two options for rewards on [https://app.openworld.vision/#/earn](https://app.openworld.vision/#/earn): "Compound" and "Claim".

Compounding will stake your pending Multiplier Points and Escrowed OpenWorld rewards, this will increase the amount of rewards you receive.

Claiming will transfer any pending Escrowed OpenWorld rewards and ETH / AVAX rewards to your wallet.

If you compound or stake your Escrowed OPEN tokens, you can unstake them for vesting at any time later on.

## Escrowed OPEN

Escrowed OPEN (esOPEN) can be used in two ways:

1. Staked for rewards similar to regular OPEN tokens
2. Vested to become actual OPEN tokens over a period of one year

Each staked Escrowed OPEN token will earn the same amount of Escrowed OPEN and ETH / AVAX rewards as a regular OPEN token.

Note that Escrowed OPEN (esOPEN) is not meant to be transferrable unless you are doing a [full account transfer](https://app.openworld.vision/#/begin\_account\_transfer). The amount of OPEN or OLP required to vest esOPEN is unique per account and capped to the rewards received by that account. Please do not buy esOPEN off the market or OTC as you will not be able to vest them.

## Vesting

Escrowed OPEN (esOPEN) tokens can be converted into OPEN tokens through vesting, this can be accessed on the [Earn](https://app.openworld.vision/#/earn) page.&#x20;

When vesting is initiated, the average amount of OPEN or OLP tokens that was used to earn the esOPEN rewards will be reserved.

For example, if you staked 1000 OPEN and earned 100 esOPEN tokens, then to vest 100 esOPEN tokens, 1000 OPEN tokens will be reserved. To vest 50 esOPEN, 500 OPEN tokens will be reserved. Note that this is an example and the actual ratio depends on the average staked amount and rewards earned for your account.

esOPEN tokens that have been unstaked and deposited for vesting will not earn rewards. Staked tokens that are reserved for vesting will continue to earn rewards.

After initiating vesting, the esOPEN tokens will be converted into OPEN every second and will fully vest over 365 days. esOPEN tokens that have been converted into OPEN are claimable at any time.

If a user sells OPEN or OLP tokens and would like to vest their esOPEN rewards later on, they would need to re-buy the OPEN or OLP tokens. OPEN, esOPEN and Multiplier Points can be used interchangeably for the required reserve amount.

Depositing into the vesting vault while existing vesting is ongoing is supported.

Tokens that are reserved for vesting cannot be unstaked or sold. To unreserve the tokens, use the "Withdraw" button on the [Earn](https://app.openworld.vision/#/earn) page. Partial withdrawals are not supported, so withdrawing will withdraw and unreserve all tokens as well as pause vesting. All esOPEN tokens that had been vested into OPEN will remain as OPEN tokens.

## Multiplier Points

Multiplier Points reward long term holders without inflation.

When you stake OPEN, you receive Multiplier Points every second at a fixed rate of 100% APR. 1000 OPEN staked for one year would earn 1000 Multiplier Points.

Multiplier points can be staked for fee rewards by pressing the "Compound" button on the [Earn](https://app.openworld.vision/#/earn) page, each multiplier point will boost ETH / AVAX APRs at the same rate as a regular OPEN token.&#x20;

When OPEN or Escrowed OPEN tokens are unstaked, the proportional amount of Multiplier Points are burnt. For example, if 1000 OPEN is staked and 500 Multiplier Points have been earned so far, then unstaking 300 OPEN would burn 150 (300 / 1000 \* 500) Multiplier Points. The burn will apply to the total amount of Multiplier Points which includes both staked and unstaked Multiplier Points.

To transfer staked tokens without burning Multiplier Points, use the Transfer button on [https://app.openworld.vision/#/earn](https://app.openworld.vision/#/earn).

The "Boost Percentage" shown on the [Earn](https://app.openworld.vision/#/earn) page shows your individual boost amount from Multiplier Points. For example, if the ETH APR is 10% and you have $10,000 worth of OPEN and esOPEN, then your rewards would be $1000 annualized, if you additionally have an amount of Multiplier Points equivalent to 20% of your total amount of OPEN and Escrowed OPEN, your "Boost Percentage" would display as 20%, and you would get an extra $200 of ETH rewards annualized. The “Boost Percentage” is calculated from the ratio of Multiplier Points to your total amount of staked OPEN:

Boost Percentage = 100 \* (Staked Multiplier Points) / (Staked OPEN + Staked esOPEN)

An example:

100 \* (4.5656) / (7.54 + 2.00) = 47.85%

![](broken-reference)

## Distribution Rate

Escrowed OPEN will be distributed to staked OPEN and OLP according to the schedule in the latest [snapshot vote](https://snapshot.org/#/openworld.eth/proposal).

Rewards are distributed every second to staked tokens.

Reward rates will be evaluated each month and may be subjected to changes. Any modifications will be announced at least 7 days in advance before being implemented.

## Summary

A summary of rewards and mechanics:

* OPEN: earns ETH / AVAX, esOPEN, Multiplier Points when staked
* esIOPEN: earns ETH / AVAX, esOPEN, Multiplier Points when staked
* Multiplier Points: boost ETH / AVAX APRs when staked
* OLP: earns ETH / AVAX, esOPEN, automatically staked on mint

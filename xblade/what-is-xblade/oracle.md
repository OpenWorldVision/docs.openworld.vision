# Oracle

## Purpose

The price oracle imperatively targets to bring the xBlade payout gained by combat as well as minting and reforging fees into line with the current dollar value of xBlade

This indicates that if the dollar value per xBlade rises, the following will happen:

* xBlade payouts falls down
* xBlade required for Mint Characters decreases
* xBlade required for Mint Weapons decreases
* xBlade required for Reforge decreases

In the event that the price of xBlade in dollar falls below a threshold, xBlade payouts and requirements will increase.

The oracle ensures that if players win a majority of their daily fights, they will earn more xBlade which is enough to pay for gas fee costs.

Depending on the changes in the dollar value of xBlade, the Oracle will dynamically adjust fight payouts up or down.

## Reason

The purpose of using Oracle is to withhold the value of in-game currency at a fixed cost. There appears to be a stipulation for the amount of xBlade token circulating in the economy. For that reason, a remarkable increase in the number of users results in an outflow of all xBlade in the contract.

Thanks to the oracle, CryptoWar creates an interrelationship between active users and the currency value of xBlade. Assuming that xBlade price increases, the demand for xBlade will increase, owing to specimen of new game features or an influx of new players.

The oracle empowers the fight transaction fees as well as minting fees for NFTs to be kept at a constant-dollar value, which permits new players to engage in the game with an affordable entrance fees even if the dollar value of xBlade rises.

## Obtaining Oracle xBlade/Dollar Rate

The Oracle follows the current dollar value of xBlade and changes xBlade price accordingly at an undisclosed rate to keep everything fair and unbiased between all players.

Cryptowar is using Pancake Price Feed oracle. To check xBlade price:&#x20;

* Go to the [PancakeSwap xBlade page](https://pancakeswap.finance/swap?inputCurrency=0x27a339d9b59b21390d7209b78a839868e319301b\&outputCurrency=0xe9e7cea3dedca5984780bafc599bd69add087d56)
* Fill value 1 into xBlade

![](<../../.gitbook/assets/Screen Shot 2021-10-23 at 12.13.42 AM.png>)

When the calculated amount is different from the actual dollar value of xBlade, buffs to payouts and mint costs are expected if the Oracle is above the current value of xBlade, and vice versa, nerfs if below.

---
description: OLP is the platform's liquidity provider token.
---

# OLP

### Overview <a href="#overview" id="overview"></a>

OLP consists of an index of assets used for swaps and leverage trading. It can be minted using any index asset and burnt to redeem any index asset. The price for minting and redemption is calculated based on (the total worth of assets in index including profits and losses of open positions) / (OLP supply).For Arbitrum, holders of the OLP token earnEscrowedOLPrewardsand 70% of platform fees distributed in ETH. For Avalanche, holders of the OLP token earnEscrowedOLPrewardsand 70% of platform fees distributed in AVAX. Note that the fees distributed are based on the number after deductingreferral rewardsand the network costs ofkeepers, keeper costs are usually around 1% of the total fees.Staked OLP token address (Arbitrum):0x1aDDD80E6039594eE970E5872D247bf0414C8903​Staked OLP token address (Avalanche):0x9e295B5B976a184B14aD8cd72413aD846C299660​Note that OLP is specific to the network you mint it on, it is not directly transferrable between networks and the price/rewards to the tokens will differ between networks.As OLP holders provide liquidity for leverage trading, they will make a profit when leverage traders make a loss and vice versa. Past PnL data, OLP price chart, and other stats can be viewed athttps://stats.gmx.io.Minting and RedeemingMinting OLP

* Bridge any of the OLP tokens to Arbitrum / Avalanche, a list of OLP tokens can be found on the [Dashboard](https://app.gmx.io/#/dashboard).
  * Fees will be lower for tokens that the pool has less of, check the "[Save on Fees](https://app.gmx.io/#/buy\_glp)" section to get the lowest fees
  * You should buy the token with the lowest fees from Ethereum and then bridge that token directly as these tokens are likely more expensive to purchase on Arbitrum
* For Arbitrum, ensure that some ETH is bridged over as you need it to pay for the network fees
  * Bridging to Arbitrum: [https://arbitrum.io/bridge-tutorial/](https://arbitrum.io/bridge-tutorial/)​
* For Avalanche, ensure that you have some AVAX for network fees
  * ​[https://bridge.avax.network/](https://bridge.avax.network/)​
* Key in the amount of OLP you'd like to purchase on: [https://app.gmx.io/#/buy\_glp](https://app.gmx.io/#/buy\_glp)​

Fees for buying OLP will vary based on which assets the index has less or more of, the Buy OLP page will show which assets have the lowest fee.After buying your tokens will automatically be staked and you will start earning Escrowed OPEN and ETH / AVAX rewards, you can check your rewards at [https://app.gmx.io/#/earn](https://app.gmx.io/#/earn).**Redeeming OLP**Key in the amount of OLP you'd like to redeem at [https://app.gmx.io/#/buy\_glp#redeem](https://app.gmx.io/#/buy\_glp#redeem). Note that there is a minimum holding time of 15 minutes after minting before you can redeem OLP tokens.

### Rebalancing <a href="#rebalancing" id="rebalancing"></a>

The fees to mint OLP, burn OLP or to perform swaps will vary based on whether the action improves the balance of assets or reduces it. For example, if the index has a large percentage of ETH and a small percentage of USDC, actions which further increase the amount of ETH the index has will have a high fee while actions that reduce the amount of ETH the index has will have a low fee.The token weights can be seen on the [Dashboard](https://app.gmx.io/#/dashboard).Token weights are adjusted to help hedge OLP holders based on the open positions of traders. For example, if a lot of traders are long ETH, then ETH would have a higher token weight, if a lot of traders are short, then a higher token weight will be given to stablecoins.If token prices are increasing, then the price of OLP will increase as well, even if a lot of traders have a long position on the platform. The portion reserved for long positions can be treated as stable in terms of its USD value since if prices increase the profits from that portion will be used to pay traders, and if prices decrease, the losses of traders will keep the USD value of the reserve portion the same.If a lot of traders are short and larger weights are given to stablecoins, then OLP holders would have a synthetic exposure to the tokens being shorted, e.g. if ETH is being shorted then the price of OLP will decrease if the price of ETH decreases if the price of ETH increases then the price of OLP will increase from the losses of the short positions.

### Risks <a href="#risks" id="risks"></a>

Caution should be exercised when interacting with any smart contract or blockchain application. While risks are attempted to be mitigated through testing, audits, and bug bounties, there is always a risk of vulnerabilities in smart contract code.For details of contract operation please read the [Contracts](https://app.gitbook.com/s/fIU6S055TNsNeN5h66Fd/olp) section.

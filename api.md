# API

For contract interaction: https://gmxio.gitbook.io/gmx/contracts.&#x20;

The URLs below are for Arbitrum, for Avalanche the same URLs are available, with the base URL being https://gmx-avax-server.uc.r.appsp



## **Tokens**

* URL: [https://api.gmx.io/tokens](https://api.gmx.io/tokens)
* Retrieve a list of tokens and info for each token
* USD amounts are multiplied by (10 \*\* 30)
* Token amounts are multiplied by (10 \*\* token. decimals)

## **Prices**

The tokens endpoint will return the current prices in the contract, these prices are used for swaps, OLP minting / redeeming. For opening and closing positions, the [realtime median prices](https://gmx-io.notion.site/GMX-Technical-Overview-47fc5ed832e243afb9e97e8a4a036353) are used, to get these values:

* URL: [https://api.gmx.io/prices](https://api.gmx.io/prices)
* Retrieve a list of token prices
* Prices are multiplied by (10 \*\* 30)

## **Actions**

* URL: [https://api.gmx.io/actions](https://api.gmx.io/actions)
* Retrieve a list of actions, these will include swaps, increasing a position, decreasing a position, orders and liquidations
* Params:
  * account (optional): pass in the checksum address of an account
  * after (optional): for pagination, the id to start after
* To get the checksum address: [https://web3-tools.netlify.app/](https://web3-tools.netlify.app/), you can also use a library like [ethers](https://docs.ethers.io/v5/)

## **Volume**

* Hourly: [https://api.gmx.io/hourly\_volume](https://api.gmx.io/hourly\_volume)
* Daily: [https://api.gmx.io/daily\_volume](https://api.gmx.io/daily\_volume)
* Weekly: [https://api.gmx.io/weekly\_volume](https://api.gmx.io/weekly\_volume)
* Total: [https://api.gmx.io/total\_volume](https://api.gmx.io/total\_volume)
* Volumes are separated by action, token, day / week
* Params:
  * after (optional): for pagination, the id to start after

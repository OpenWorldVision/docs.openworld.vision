# Marketplace

When engaging in the game, players possess their own assets for example characters & weapons which are stockpiled in the game and minted in ERC-721 NFTs. These assets can be freely traded with other players. All in-game transactions are conducted on an exclusive marketplace owned by CryptoWar in which players are granted permission to enlist and purchase their NFTs for eliminating massive frauds while doing trades through the use of NFT contracts.

## Approving xBlade Spending

After purchasing NFTs on the marketplace, the system automatically dispatch a notification of a transaction approval form to the players, as illustrated in the following photo:

It is due to the fact that CryptoWar is not given authorization to spend xBlade directly from players’ MetaMask wallet. Consequently, players are obligated to seek authorization whenever they need to execute a marketplace transaction, which appears to be completely different from the actual purchase confirmation. After the completion of transaction approval, players will receive an official notification of purchasing process on the market.

![](<../.gitbook/assets/11 (1) (1).jpg>)

{% hint style="info" %}
It is advisable to have a strategic purchase planning for each item on the market; otherwise players will receive a gas fee error in case they try out for items purchased by someone else.
{% endhint %}

## Tax

To list an NFT, a certain amount of gas fee will be requested to execute in-game transactions for the purpose of transferring NFT to the marketplace contract.

The tax charged on purchasing NFT on the marketplace is at the rate of 10% which is paid by the buyers. For each purchasing transaction on the marketplace, tax is included in the listed price of NFTs and the 10% tax is redirected to the contract in so as to pay for xBlade through combat.

## Trade Lock

Characters listed and bought via the marketplace or traded via smart contracts will be locked within 24 hours before the item is enabled to be listed or traded again.

{% hint style="info" %}
0.285 gas fee errors will be charged on making constant effort to list or trade a locked item. Please do not perform any transaction during this time.
{% endhint %}

## Browse NFTs

![image](https://github.com/ElasticBTC-XBT/CryptoWar-Wiki/tree/534c0aa13bb170622866cfb21d20deb8b8953046/.gitbook/assets/browse-nfts.png)

The Browse NFTs tab empowers players to overlook existing characters and weapons. Click on “Filter button” in case players want to short-list available options for both characters and weapons. Due to the lack of pagination, only the first 60 results will be displayed in the research results. Players are required to obtain the asset ID and paste it into Search NFTs as illustrated in the following picture in case they seek to make a direct purchase of someone’s listed NFT on the marketplace.

## Search NFTs

![image](https://github.com/ElasticBTC-XBT/CryptoWar-Wiki/tree/534c0aa13bb170622866cfb21d20deb8b8953046/.gitbook/assets/search-nfts.png)

If players are able to access to the asset ID of the NFT purchased or to the sellers’ wallet, they may overlook them directly under the Search NFTs tab.

After that, simply paste asset ID on the textbox and select either "Search Character ID" or "Search Weapon ID" to detect players’ wanted NFT.

In case players have the seller’s wallet address, they may possibly insert it into the textbox and choose “Characters by Seller” or “Weapons by Seller” to see over all of their existing characters and weapons. What is more, players can use this tab to keep track of their current characters and weapons, along with their tax-inclusive price.

Players are empowered to de-list the item or adjust its’ listed price when selecting a listed NFT. Nevertheless, it is worth noting that players should place a new price into the textbox after the process of adjusting price, which will then be taxed at the rate of 10% before having the item re-listed on the marketplace.

{% hint style="info" %}
It is important to keep in mind that delisting an item leads to 24-hour trading lock. For that reason, players are advised not to engage in any trades or re-list the item.
{% endhint %}

## List NFTs

![image](https://github.com/ElasticBTC-XBT/CryptoWar-Wiki/tree/534c0aa13bb170622866cfb21d20deb8b8953046/.gitbook/assets/list-nfts.png)

Players can list their own NFTs on the marketplace using the List NFTs tab. The price they are trying to earn from selling their NFTs will have a 10% tax added on top of it to become the listed price. After their listings, their listed NFTs will be transferred to the marketplace and their slots in players’ wallet will be freed up for minting new NFTs. De-listing will return the NFTs to their slots in players’ wallet unless they are full (in which case the de-listing will be unavailable). Please note that listing will incur a gas fee similar to trading. CryptoWar will also ask for players’ permission to use their CBC or CBW.

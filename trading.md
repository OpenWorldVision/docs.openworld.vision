# Trading





**Adding a wallet**

In order to trade on OpenWorld you need crypto wallet extension on your web browser. If you do not have a wallet yet, you can use MetaMask:[https://metamask.io/download/](https://metamask.io/download/)

Then, you add the BNB Chain network to your MetaMask:[https://academy.binance.com/en/articles/connecting-metamask-to-binance-smart-chain](https://academy.binance.com/en/articles/connecting-metamask-to-binance-smart-chain)

**Sending tokens**

You will need to have BNB in your BNB Chain Metamask Account to start trading.

We are working with Stably so that you can buy BNB directly from your bank account. We will update this later.

Besides, you can buy BNB from PancakeSwap:[https://pancakeswap.finance/](https://pancakeswap.finance/) and use the BNB to pay gas fee when you trade on OpenWorld.

Opening a Position

You can trade long or short depending on which side you would like to take on the market.

With a long position, you make a profit when the market price goes up and you make a loss when the market price goes down. With a short position, you make a profit when the market price goes down and you make a loss when the market price goes up.

After taking your side, key in the amount you want to pay and the leverage you want to use, in the example we have here, \[Alec key in] worth \[Alec key in] is being used to buy \[Alec key in] long position at the size of \[Alec key in].

The “Entry Price” is \[Alec key in] and the Liquidation Price is \[Alec key in]. Below the swap box you also see the “Exit Price”, which is the price that would be used to calculate profits (or loss) if you close a position.

Managing Positions

After opening a trade, you can view it under your Position tab, you can also “Edit” to deposit or withdraw collateral, this allows you to manage your leverage and liquidation price.

When you open a position or deposit collateral, a snapshot of the USD price of your collateral is taken, so if your collateral is \[Alec to key in] and the price of \[Alec to key in] at the time, then your collateral is \[Alec to key in] and will not change even if the price of \[Alec to key in] changes.



The amount of profit and loss you make will be proportional to your position size. In this example, \[Alec to key in] has been used to buy \[Alec]. If the price of \[Alec] increase by 10%, the position would have a profit of \[Alec]. If the price of \[Alec] to decrease by 10%, the position would have a loss of \[Alec].



Leverage for a position is displayed as (position size) / (position collateral). If you'd like to display the leverage as (position size + PnL) / (position collateral), you can customise this by clicking on the "..." button next to your address.

Note that when depositing collateral into a long position, there is a 0.3% swap fee for the conversion of the asset to its USD value. This is to prevent deposits from being used as a zero fee swap. This does not apply to shorts. Withdrawing of collateral from longs and shorts do not have this fee as well.

When you make the trade, even though due to this is derivative market and your order don’t move price on the spot market, there can be slippage due to price movements in the market from when your trade is submitted to when it is confirmed on chain. Slippage might happen. Slippage is the difference between the expected price of the trade and the execution price, this can be customised by clicking on the "..." icon next to your address at the top right of the page.

Closing a Position

To close a full position or partially a position, click on “Close” button.

For long positions, profits are paid in the asset you go long. For example, if you long ETH, you would get profits as ETH. For short positions, profits will be paid in the same stablecoin that you use to go short.

Stop-Loss / Take-Profit Orders

You can also set stop-loss and take-profit orders by clicking on the “Close” button and selecting the “Trigger” tab.

After creating a trigger order, it will appear in your position's row as well as under the "Orders" tab, you can edit it the order and change the trigger price if needed.

If you close a position manually, the associated trigger orders will remain open, you would need to cancel them manually if you do not want the order to be active when the market price hit your trigger price and opening future positions.

Note that orders are not guaranteed to execute, this can occur in a few situations including but not exclusive to:

* The mark price which is an aggregate of exchange prices did not reach the specified price
* The specified price was reached but not long enough for it to be executed
* No keeper picked up the order for execution

Additionally, trigger orders are market orders and are not guaranteed to execute at the trigger price.

Partial Liquidations

In the example, since only \[Alec] worth of tokens is used as collateral to open the position, there will be a price at which the loss amount is very close to the collateral amount, which will trigger liquidation.

The Liquidation Price and is calculated as the price at which the (collateral - losses - borrow fee) is less than 1% of your position's size. If the token's price crosses this point then the position will be automatically closed.

Due to the borrow fee your liquidation price will change over time, especially if you use a leverage that is more than 10x and have the position open for more than a few days, so it is important to monitor your liquidation price.

If there is any collateral remaining after deducting losses and fees, then the corresponding amount would be returned to your account.

Pricing

There is no price impact for trades on OpenWorld, so you can execute large trades exactly or very close to the mark price. During times of high volatility there will be a spread from the Chainlink price to the median price of reference exchanges.

The mark prices are displayed next to the market name, long positions will be opened at the higher price and closed at the lower price while short positions will be opened at the lower price and closed at the higher price.

The chart will indicate the average of the two mark prices.

Fee

The trading fee to open a position is 0.05% of the position size. Similarly, there is a 0.05% trading fee when you close a position.

There is also a "Borrow Fee" that is deducted to your position at the start of every hour. This is the fee paid to the capital provider of your trade (OAP). The fee per hour changes from utilization of the capital by market participants, the formula is: (assets borrowed) / (total assets in pool) \* 0.01%. The "Borrow Fee" for longing or shorting is shown below the swap box.

The collateral of long positions is the token being longed, for example, ETH longs the collateral is ETH. The collateral of shorts positions is any of the supported stablecoins e.g. BUSD, USDC, etc. If a swap is needed when opening or closing a position then the regular swap fee would apply, this fee is 0.2% to 0.8% of the collateral size.

There are two transactions involved in opening / closing / editing a position:

* User sends the first transaction to request open / close / deposit collateral / withdraw collateral
* Keepers observe the blockchain for these queries and execute them

The cost of the second transaction is displayed in the confirmation box as the "Execution Fee". This network cost is paid to the blockchain network.

---
description: List of OPEN contracts.
---

# Contracts

## Staking

The RewardRouter contract handles the necessary actions needed for staking in a single transaction.

When staking OPEN:

* The RewardRouter deposits the OPEN token into the StakedOpenTracker contract
* The StakedOpenTracker issues itself as a token for each token deposited
* esOPEN can similarly be deposited into the StakedOpenTracker
* The StakedOpenTracker distributes esOPEN to staked tokens
* After this step, the RewardRouter deposits the StakedOpenTracker tokens into the BonusOpenTracker
* The BonusOpenTracker distributes Multiplier Points to staked tokens
* Finally the BonusOpenTracker tokens are deposited into the FeeOpenTracker which distributes ETH or AVAX to staked tokens

When minting OLP:

* The RewardRouter sends the funds to be deposited to the OlpManager and mints OLP tokens
* The RewardRouter then deposits the OPEN tokens to the FeeOlpTracker which distributes ETH or AVAX to the staked tokens
* Finally the RewardRouter deposits the FeeOlpTracker tokens into the StakedOlpTracker which distributes esOPEN to staked tokens

Addresses for contracts can be found at [https://github.com/OpenWorldVision](https://github.com/OpenWorldVision)

To get the deposit balances for an account you can use RewardTracker.depositBalances(account, token), or RewardReader.getDepositBalances(account, depositTokens, rewardTrackers).

To get claimable rewards you can use RewardReader.getStakingInfo(account rewardTrackers), this returns an array of uint256 values in the order:

* Claimable rewards
* Amount of reward token distribution per second
* Average staked amount for account
* Total rewards distributed to account
* Total staked tokens in the rewardTracker

## Testnet Deployments

The below contracts were deployed on the Arbitrum Testnet before [http://arbiscan.io](http://arbiscan.io/) was available, note that they are not actively maintained:

* Vault: [0xA4704fBfaf7c89511668052931Ba0f1816D2c9d3](https://testnet.arbiscan.io/address/0xA4704fBfaf7c89511668052931Ba0f1816D2c9d3)
* Router: [0x526f42EA12E167E36E3De747187f53b6989d121A](https://testnet.arbiscan.io/address/0x526f42EA12E167E36E3De747187f53b6989d121A)

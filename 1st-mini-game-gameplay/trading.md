# Trading

It appears that players may freely perform in-game transactions with one another outside the marketplace via the use of NFT smart contracts thanks to their own NFT assets. Trading characters by using NFT smart contracts may lead to 24-hour trading lock.

{% hint style="info" %}
Players should be aware that there are safety risks for players to make themselves a victim of scams or frauds when executing peer-to-peer transactions. Under no circumstance will CryptoWar team accept responsibility for any loss on players’ xBlade or NFTs in case they conduct peer-to-peer trade. For that reason, it is advisable that players had better carry on in-game transactions on CryptoWar marketplace in order to keep their trading secured.
{% endhint %}

## Trading Characters

The character contract, which can be explored on the link below, is used to trade characters. It is worth noting that character contract is completely different from weapon contract. Further information on the character contract can be found here: [**CryptoWar Character Trading Contract**](https://bscscan.com/address/0xC38470BFE1b08c3baFDaf699eBa2fCA1fd2B040B#writeProxyContract) ****&#x20;

0xC38470BFE1b08c3baFDaf699eBa2fCA1fd2B040B&#x20;

{% hint style="info" %}
Players are warned to be on the alert for not trading weapons on the character contract.
{% endhint %}

Please ensure that players’ receiving wallet has an extra character slot and the character in question is not trade locked to properly conduct transactions. If everything is perfectly aligned, follow the instructions below:

1. Click on "Connect to Web3" as shown in the picture below and connect your MetaMask.

![image](https://user-images.githubusercontent.com/90205972/136993577-fb30e73c-ac5c-4c66-b9e8-fe607bb76b51.png)

1. Go to “Function 11- safeTransferFrom” and input the following data:

* “from (address)” means the owner’s address
* “to (address)” refers to the receiver’s address
* “tokenID (uint256)” is the Character ID
*

1. Tab on "Write". The verification will be sent directly to your account by MetaMask to confirm your transaction.
2. Pay the gas fee and wait for your transaction to complete.

{% hint style="info" %}
Please note that the character’s account is the one connected to the contract
{% endhint %}

## Trading Weapons

The weapon contract, which can be viewed on the link below, is only applied to trade weapon. It is worth noting that weapon contract is completely different from character contract, empowering players to only trade weapons.

Further information on the weapon contract can be discovered here: [**CryptoWar Weapon Trading Contract**](https://bscscan.com/address/0x52683412f6Ea2B6302ceA8406EfF928510466c2c#writeProxyContract)****

0x52683412f6Ea2B6302ceA8406EfF928510466c2c

{% hint style="info" %}
Players are warned to be on the alert for not trading characters on the weapon contract.
{% endhint %}

Players are expected to follow the same instructions as they have done for the character contract.

1. Click on "Connect to Web3" as shown in the picture below and connect your MetaMask.

![image](https://user-images.githubusercontent.com/90205972/136999644-d6fe3f97-fb3b-4b20-bef9-353f3427c17d.png)

1. Go to “Function 17- safeTransferFrom” and input the following data:

* “from (address)” means the owner’s address
* “to (address)” refers to the receiver’s address
* “tokenID (uint256)” is the Weapon ID

1. Click on "Write". You will be prompted by MetaMask to confirm your transaction.
2. Pay the gas fee and wait for your transaction to complete.

{% hint style="info" %}
Please note that the character’s account is the one connected to the contract.
{% endhint %}

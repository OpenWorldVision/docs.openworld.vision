# Calculating Power

## Unaligned Character Power

Unaligned Character Power is the variable used to determine the range of enemy power rolls.

The following are the variables needed to calculate this:

|                           |   |                                                                                                                                                 |
| ------------------------- | - | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Variable**              | . | **Description**                                                                                                                                 |
| **Character Power**       | . | **Character Power** is the listed power displayed on the upper left hand side of the screen above the stamina bar when a character is selected. |
| **Weapon Attribute Base** | . | **Weapon Attribute Base** is the sum of all the weapon's attribute values without taking elemental matching into account.                       |
| **Weapon Bonus Power**    | . | **Weapon Bonus Power** is the specified bonus power value if the weapon has been reforged.                                                      |

Unaligned power is currently calculated using the following formula:

$$
unalignedPower = (((attributeTotal * 0.0025) + 1) * charPower) +bonusPower
$$

After calculating unaligned power, we do a ±20% multiplier to estimate the range of enemy power values.

{% hint style="info" %}
Let's take another calculating sample using the following values:

* Character Power - 1000 (a level one character)
* Attribute Total - 800 (a max attribute 4-star weapon)
* Bonus Power - 1500 (a 100/100 LB, 0/25 4B, 0/10 5B weapon)

Unaligned Power is up to 4500.

4500 \* 0.8 rounded to the nearest whole number is 3600 which is Minimum Enemy Power.

4500 \* 1.2 rounded to the nearest whole number is 5400 which is Maximum Enemy Power.
{% endhint %}

## Aligned Character Power

In conjunction with Trait Bonus, Aligned Character Power is employed to determine the player’s combat roll.

The variables needed for Aligned Character Power’s calculation result are analogous to those of Unaligned Character Power mentioned above. The difference is that the game uses Aligned Character Power instead of Unaligned Character Power to perform the calculation.

|                           |   |                                                                                                         |
| ------------------------- | - | ------------------------------------------------------------------------------------------------------- |
| **Weapon Attribute Base** | . | **Weapon Attribute Base** is the sum of all the weapon's attribute values excluding elemental matching. |

Aligned Character Power uses

|                                 |   |                                                                                                                                                                                 |
| ------------------------------- | - | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Weapon Attribute Multiplied** | . | **Weapon Attribute Multiplied** is the sum of all the weapon's attribute values after providing multiply-accumulate computation for each attribute based on elemental matching. |

We purpose to evaluate each attribute discretely and use the following formulas to calibrate its value in lieu of having the formula simply added up to all the weapons’ attributes.

```
if attributeElement != charElement (attributeValue * 0.0025)
if attributeElement == PWR (attributeValue * 0.002575)
if attributeElement == charElement (attributeValue * 0.002675)
```

Each weapon’s attribute is summed up in the similar formula as unaligned power to collar the aligned power after having each attribute been evaluated.

$$
alignedPower = ((evaluatedAttributeTotal + 1) * charPower) + bonusPower
$$

{% hint style="info" %}
Let's take another calculating sample using the following values:

* Character Power - 1000 (a level one character)
* Character Element - Fire
* Attribute One - STR 400
* Attribute Two - CHA 400
* Bonus Power - 1500 (a 100/100 LB, 0/25 4B, 0/10 5B weapon)

Aligned Power is up to 4570.
{% endhint %}

Aligned Power is employed to estimate experience obtained, which is then compounded to multiply with Trait Bonus for further calculation of player’s combat roll.

## Trait Bonus

Trait Bonus is a variable that is multiplied by Aligned Power to determine the player’s combat roll.

The formula to calculate Trait Bonus is shown below:

![](../../.gitbook/assets/13.jpg)

![](<../../.gitbook/assets/12 (1) (1).jpg>)

```
TraitBonus = 1
if charElement == weaponElement (TraitBonus += 0.075)
if charElement > enemyElement (TraitBonus += 0.075)
if charElement < enemyElement (TraitBonus -= 0.075)
```

The following are instructions about character elements to get the upper hand of your enemy:

* Fire beats Earth
* Earth beats Air
* Air beats Water
* Water beats Fire

![](<../../.gitbook/assets/14 (1) (1).jpg>)

The players’ final power value is totalized by measuring Trait Bonus and multiplying it by Aligned Power.

A ±20% is then applied to the final value to determine the player's combat roll, then to make the game sustainble, the final combat roll will be adjusted so that the higher level, the harder to win but earning the higher reward when win.

{% hint style="info" %}
The following variables are assumed based on the Aligned Power calculated above.

* Character Element - Fire
* Weapon Element - Water
* Enemy Element - Earth

Trait Bonus is up to 1.075.

The Final Power Value comes down to 4912 after adding Trait Bonus to the Aligned Power mentioned above.

4912 \* 0.9 rounded to the nearest whole number is 4420 which is Minimum Player Roll.

4912 \* 1.1 rounded to the nearest whole number is 5403 which is Maximum Player Roll.
{% endhint %}

## Enemy Power

Enemy Power is considered to be a straightforward ±20% calculation used to measure the power of whichever of enemy each player selected from the listed enemy power.

Experience and xWeapon payouts can be identified by means of checking over the numerical value listed on the combat screen button.

The estimated value with the ±20% applied is used to determine the enemy's rolls in combat:

{% hint style="info" %}
To make it more explicit to the players, let’s run a combat simulation by taking the preceding values into account:

* Minimum Enemy Power = 4050
* Maximum Enemy Power = 4950

Assuming that the player chose an enemy with a listed power value of 4700:

* Enemy Power = 4700

4700 \* 0.9 rounded to the nearest whole number is 4230 which is Minimum Enemy Power.

4700 \* 1.1 rounded to the nearest whole number is 5170 which is Maximum Enemy Power.

Given the results of our simulation, we can conclude that the player can roll between 4420-5403 while the enemy can roll between 4230-5170.
{% endhint %}

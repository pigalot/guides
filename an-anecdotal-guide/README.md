# An Anecdotal Guide

To Adventure Land (An Indie Coding MMO)

*Written by **Aria Harper**. Converted from the "An Anecdotal Guide v3.0" PDF; wording is the
author's, with the original footnotes kept at the bottom.*

## Contents

- [Foreword](#foreword)
- [Upgrading](#upgrading)
  - [The Basics](#the-basics) · [Grade](#grade) · [Scrolls](#scrolls) · [Offerings](#offerings)
  - [Details](#details) — [Chances](#chances), [Grace](#grace), [Karma](#karma), [Lucky Slot](#lucky-slot), [Beyond the Upgrade Cap](#beyond-the-upgrade-cap)
  - [Techniques](#techniques) — [Prim Stacking](#prim-stacking), [Horizontal Upgrading](#horizontal-upgrading), [Failstacking](#failstacking), [Abandon All Hope](#abandon-all-hope), [Ratchet Upgrading](#ratchet-upgrading), [Numb](#numb)
- [Compounding](#compounding)
  - [Scrolls](#scrolls-1) · [Techniques](#techniques-1) — [Patience](#patience), [Failstacking](#failstacking-1), [Horizontal Compounding](#horizontal-compounding)
- [Drops](#drops)
  - [The Basics](#the-basics-1) — [Luck](#luck), [Gold](#gold)
  - [Details](#details-1) — [Monster Drops](#monster-drops), [Map Drops](#map-drops), [Global Drops](#global-drops), [Monster Leveling](#monster-leveling), [Ordering](#ordering), [Special Cases](#special-cases)
- [Party and Co-op](#party-and-co-op)
- [Properties](#properties) — [Obtainment](#obtainment), [Shiny](#shiny)

---

## Foreword

This guide is from a personal perspective. Everything in here is based upon my own observations. As such, everything contained within is anecdotal. However, I have no reason to deceive you. Many of the mechanics described herein are obscure, and are not even official. However, I have found them all to be true, at least in my own experience.

Since the game's open-source, we have found many of the mechanics described in previous versions of this document to be correct. Other mechanics were completely unknown, such as the Lucky Slot. Others were suspected, but never confirmed prior to open-source, and as such were never mentioned in earlier versions of this document.

Names used here are not official, nor should you treat them as such. I have simply named them to the best of my ability, based on their effects.

You need not read the entirety of this guide. If you think you understand the mechanics well enough, then feel free to not read on them. However, there are some gems in here that not even some of the experienced players know - or at the very least, they thought them odd.

I have avoided using numbers as much as I can. Numbers are bound to change, but their relationships are not. While an item's damage may change, the more it is upgraded, the more damage it deals. Such is my philosophy when discussing mechanics.

Now that you have a better idea of the information you will find, feel free to read onwards. I hope you learn something new, at the very least. If not, I hope my observations align with your own, and that my information is accurate. Enjoy!

---

## Upgrading

One of the most important mechanics in the game is upgrading. Upgrading is how you progress through the entirety of the game. Some of the mechanics of Upgrading are not well understood, and are still obscure.

### The Basics

Upgrading at the very core involves 2 things: An item, and a scroll. When an item is upgraded, the scroll is consumed, and the dice roll. The 4 numbers at the top determine the chance of success. When the dice are rolled, the result has to be less than the 4 top numbers in order for the upgrade to succeed. If the upgrade succeeds, the item's level is incremented. If the upgrade fails, the item is destroyed.[^1]

A common question is whether Luck (In particular, the stat) affects upgrade chances. To put it simply, it does not affect the chance displayed. Whether or not it affects the generated roll, we do not know.

### Grade

An item has a grade, and the grade is commonly associated with the item's rarity. Grades are also associated with a number range. The grades are as follows:

| Grade | Range |
| --- | --- |
| Common | 0.X |
| High | 1.X |
| Rare | 2.X |
| Legendary | 3.X |
| Exalted | 4.X |

An item's grade determines the scroll that is required to upgrade it, or the quantity of stat scrolls to change the stat points. As you upgrade an item, its grade will increase, and you will need better scrolls. An item with a decimal Grade has a stronger effect on items with a Grade below theirs, regardless of the difference in Grade. Exalted items cannot be upgraded.

### Scrolls

#### Upgrade Scrolls

There is an Upgrade Scroll for every grade, except for Exalted:

| Scroll | Grade |
| --- | --- |
| Upgrade Scroll | 0.0 |
| High Upgrade Scroll | 1.0 |
| Rare Upgrade Scroll | 2.0 |
| Legendary Upgrade Scroll | 3.0 |
| Ultimate Upgrade Scroll | 3.6 |

When using an Upgrade Scroll with a higher grade than that of the item, the chance cap for the upgrade is increased. As such, it may be worthwhile to use a higher Upgrade Scroll than required. It should be noted that it does not matter how much higher the scroll is—they all will have the same effect on the upgrade chance.

#### Stat Scrolls

There is a Stat Scroll for almost every stat. Only the primary stats (Intelligence, Strength, and Dexterity) are purchasable from NPCs. Vitality Scrolls are readily available, while Fortitude Scrolls drop from the Vampires (Mrs. and Mr. Dracul). The remainder of the Stat Scrolls are practically unobtainable, and highly coveted. An item can fail a stat change, unless an offering is provided.[^2] Additionally, the number of stat scrolls required to apply the stat to an item increases with item grade:

| Item grade | Stat scrolls required |
| --- | --- |
| Common | 1 |
| High | 10 |
| Rare | 100 |
| Legendary | 1000 |
| Exalted | 9999 |

### Offerings

Offerings are a unique class of items that pair with scrolls. By themselves, they do not destroy the item, but enhance it in some way. They can be combined with a scroll to increase the chance of success.

#### Primordial

The various primordial offerings can be used to increase the chance that an upgrade succeeds. The Primordial Offerings and their grades are as follows:

| Offering | Grade |
| --- | --- |
| Primling | 1.0 |
| Primordial Essence | 2.0 |
| Primordial X | 3.0 |

The grade of the offering determines the item grade it is most effective on. See the section on [Grade](#grade).

#### Material

Material offerings can be used to apply the Shiny attribute to an item if the item has not been upgraded, and the grade of the offering is greater or equal to the grade of the item. There are currently 3 varieties of material offering:

| Offering | Grade |
| --- | --- |
| Bronze Nugget | N/A |
| Bronze Ingot | 0.1 |
| Gold Nugget | 0.0 |
| Gold Ingot | 1.1 |
| Platinum Nugget | 1.0 |
| Platinum Ingot | 2.1 |

When applying the Shiny attribute, the item is not destroyed if it is lost. If the upgrade succeeds, the Shiny attribute is applied to the item. Material offerings can not be used on items that have been previously upgraded. They can be used as a Primordial Offering if they are combined with a scroll, but only on an un-upgraded item.

### Details

#### Chances

Many factors can affect the chance an upgrade succeeds. However, they can all be categorized into two forms: Karma, and Offering. There are also two parts to the chance: The raw value, and the chance cap. The final chance is the minimum of the two - the final value cannot exceed the cap. It should be noted that while the chance you see has only 4 digits, there are actually more, and you can fail or succeed an upgrade even if the roll matches the chance. If the upgrade succeeds, the item gets the Lucky attribute. If the upgrade fails, you are given an Essence of Greed for your loss.[^3]

The cap is influenced exclusively[^4] by the scroll and offering used in a true upgrade. A "true upgrade" is defined as any upgrade using an Upgrade scroll. Using a higher scroll than required raises the chance cap. Using an offering in a true upgrade also raises the chance cap. If the offering's grade is the same as the grade of the item, it is "qualified". If the offering's grade is higher than the item grade, it is over-qualified. Over-qualified offerings raise the cap more than a qualified offering. If the offering's grade is lower than the item grade, it is "under-qualified", and raises the cap less than a qualified offering.

If the scroll is a higher tier than required to upgrade the item, it is "over-qualified" as well, and will raise the cap comparably to a qualified offering. This effect does not stack with an "over-qualified" offering, but does stack with a "qualified" offering, producing a cap similar to an "over-qualified" offering.

The final chance is the minimum of the raw value and the chance cap. In general, you should use a qualified offering, and an over-qualified scroll, if possible. An Over-qualified scroll (i.e. Legendary Upgrade Scroll) is significantly cheaper to obtain than an over-qualified offering (i.e. Primordial X).

#### Grace

The "Grace" factor is determined by an item's actual grace property, as well as the grade of scroll and offering used in the upgrade. Grace can also be increased by using an offering, with or without a scroll. It should be noted that each individual instance of an item has its own Grace property.

#### Karma

The "Karma" factor is determined by what has recently occurred. If you fail an upgrade, Karma increases. If you succeed with an upgrade, Karma decreases. There are 2 forms of Karma: Server, and Player. Server Karma is shared between all upgrades on the current server, while Player is attached to an individual player. Negative Player Karma will lower the chance cap on an upgrade, but positive Player Karma does not raise the cap, only the raw chance value. Caution should be taken when utilizing Server Karma for upgrades, as Server Karma can fluctuate wildly as other players make their own upgrades.

#### Lucky Slot

Every character has a "lucky slot" which is determined upon the first time a character logs into a server. This slot is randomly chosen from the 42 slots in their inventory. Players may notice that upgrades in a particular slot roll lower averages than other slots, and this is likely their lucky slot. When an upgrade occurs in the lucky slot, there is a chance for it to trigger, reducing the roll used in the upgrade.[^5] This results in the slot having a higher chance to succeed most upgrades.

#### Beyond the Upgrade Cap

There is a way to get an item to a level beyond the normal upgrading capacity, and all the way to level 13. This only works on upgradeable items (not compoundables), and has an extremely low chance of succeeding.[^6] This even works on items that normally cap significantly below +Z (level 12), such as rare grade items that cap at +X (level 10). If this succeeds, the item is given to the player as a +13 item, and destroyed if it fails.

### Techniques

#### Prim Stacking

Prim(ordial) stacking uses multiple offerings to increase the Grace value of an item. This is extremely expensive, but also incredibly effective. Tens of offerings may be required. It should be noted that this only needs to be done once per item - the effect persists after an upgrade. Higher grade offerings do not increase the grace of an item more than lower grade offerings when used in Prim Stacking.[^7] As such, it is advised to use the lowest grade offering possible when Prim Stacking.

#### Horizontal Upgrading

Horizontal upgrading is when you upgrade items in layers, upgrading them all to the same level, then repeating the process. This takes advantage of Karma, getting the most out of every upgrade failure. Strongly advised, but difficult to automate.

#### Failstacking

Since failing an upgrade increases your Karma, items can be prepared before-hand that are supposed to fail their next upgrade in order to increase the player's Karma. This comes with a risk, however. If the upgrade (unexpectedly) succeeds, your Karma will be reset (It will actually be set to a negative value). While this strategy is powerful, caution should be exercised. Other players can utilize the Server Karma for their own upgrades, and if they succeed, the Server Karma will be reset.

#### Abandon All Hope

While this technique is not recommended, it is effective. Effective at what, is unclear. Since upgrading every item you have (Including current gear) does in fact mean you have more items to upgrade, and, as such, more rolls, it also means you, well, are likely to lose your gear. Many valuable items have been produced this way. Many valuable items have been lost this way. Not advised.

#### Ratchet Upgrading

Named after the indomitable device that we all know and love, Ratchet Upgrading is the opposite of Abandon All Hope. You keep an item, and if you get another, you upgrade until it is better than your current one. If it becomes better, you upgrade your current one. You continue, going back and forth, until one of them breaks. This strategy is most visible with exceedingly rare items, ones that you may only ever have two or three at a time. While this technique does not intrinsically take advantage of Karma or Grace, it is infallible in that you always have gear to use. Strongly advised early-mid game.

#### Numb

While this is less of a technique, and more of an emotional coping mechanism, it is still noteworthy. Eventually, the failures start to lose meaning, as do the successes. The grind, after all, is eternal, yet your time is finite. Strongly advised mid-late game.

---

## Compounding

The mechanics for compounding are largely the same. However, you need 3 of an item at a given level to make the next level. Additionally, there is no way to Prim Stack, as a compound cannot be partially completed. Grace does still exist, however, and is extremely powerful. After a compound, the maximum grace of the three items is used to calculate the new grace value. The Shiny attribute cannot be forced onto a compoundable item, but can be found on looted or exchanged compoundables.

### Scrolls

The scroll layout is similar for compounding:

| Scroll | Grade |
| --- | --- |
| Compound Scroll | 0.0 |
| High Compound Scroll | 1.0 |
| Rare Compound Scroll | 2.0 |
| Legendary Compound Scroll | 3.0 |

The immediate observation is that there is no Ultimate Compound Scroll. Apart from this, the scroll systems are the same.

### Techniques

#### Patience

It has been shown that an item that needs to be compounded gradually gains chance over time. While extended research into this area is not possible (simply due to the time-consuming nature of this mechanic), it has been observed to have significant results. Generally, this effect is only observed on items that are being used, i.e. worn by an active character.

#### Failstacking

Failstacking is still effective, but problematic, due to the vast resource requirements this strategy uses when used with exponential cost requirements. Not advised.

#### Horizontal Compounding

Horizontal compounding retains the efficiency, but becomes more problematic. The number of items needed to make an item of a particular level becomes exponential, instead of a constant. This analysis does not account for failure, so the expected scenario is much worse. As this method isn't extraordinarily destructive, it is advised. However, beware of the potential costs.

---

## Drops

One of the most important mechanics of any RPG-esque game is the loot. After all, the grind is only eternal because there is more loot to be had. This section will cover some of the core mechanics for drops. It should be noted that the TrackTrix can show you raw drop rates for any mob.[^8]

### The Basics

#### Luck

Luck is a linear multiplier on the stated chance of an item dropping, and items that give Luck in meaningful amounts are highly coveted.

#### Gold

Gold is a linear multiplier on the stated gold drops of a monster, and items that give Gold in meaningful amounts are highly coveted. Gold is extremely valuable on mobs that have high gold drops but no item drops, as items typically sell for more than the monster drops in gold.

### Details

#### Monster Drops

Some drops are particular to a monster. These rates are fixed, meaning that even if a mob were to change maps, it would still drop them.[^9] There is nothing special about these drops, they scale linearly with luck.

#### Map Drops

Some drops are constrained to a map. These rates are scaled linearly with a mob's maximum HP. Map drops are applied when the mob dies, so if a mob somehow changes maps, it will use the loot table from the map it died on.

#### Global Drops

Some drops are global, and are shared across all mobs on a server. There are two forms of global drops, standard and static. Static global drops have a fixed rate from every mob.[^10] Normal global drops scale with a monster's maximum HP.[^11]

#### Monster Leveling

Monsters can gain levels, just like players. When they level up, they drop more gold, and have a higher chance to drop items. Monster drop chances are affected linearly, as are static global drops. Normal global drops and map drops are affected exponentially by monster level.

#### Ordering

Luck and Gold modifiers are applied at different times. Luck is applied when the monster dies, and the luck used is that of the monster's target. If the monster was not targeting a player when it died, the luck used is that of the killer. Gold multipliers are applied when the chest is looted, and the Gold multiplier is that of the looter. Gold multiplier is applied, and then the resulting gold is split across the party.

The careful reader will note that this ordering is conducive to boosters: A booster can be kept in the luck form when a monster is about to die, shifted to the gold form, and then the chest can be looted. This can also be done with gear, in order to maximize Luck and Gold.

#### Special Cases

There are a few ways to obtain drops that don't involve killing a monster. You can heal a Ghost to get an essence of life, and you can converse with the Mainframe to get Computer Parts and the occasional Network Card. Both of these methods are unaffected by luck.

---

## Party and Co-op

Party mechanics are convoluted when they involve more than one account, and Co-op mechanics are even more convoluted, and the combination produces an abomination. Because of the sheer complexity and the fact that these two mechanics have changed frequently, and will likely change in the future, I will not attempt to explain these mechanics, but rather, note the oddities that I have seen.

### Party

When in a party with your own characters, all characters get an equal party share. As soon as another account is involved, however, party share becomes based upon various measurements of a character's "contribution". Contribution can be increased by tanking damage, dealing damage, or healing others.

### Co-op

Co-op monsters effectively create a large "party" for all players that attack it. Loot is again distributed based on contribution, but contribution is only based on damage dealt to the monster.

### Co-op & Party

Co-op monsters behave oddly when paired with a party. Given a party with 3 characters, the monster will drop 4 chests. One of the chests is for the entire party, and one is for each of the characters that damaged it (for the sake of simplicity, only 3 characters damaged the monster, all in the party).

---

## Properties

Items can have properties. These properties enhance the item in one way or another. Most properties give a particular stat, which, although weak, can add up.

### Obtainment

Most properties are obtained through achievements. Some are obtained through the upgrade system. Others can be obtained through natural chance from monster drops or exchanges.

### Shiny

The most frequently misunderstood property is Shiny. Shiny affects an item based on what type of item it is. Its priorities are as follows:

1. Weapon (has Damage)
2. Stat (has Stat)
3. Armor (has Armor)
4. Misc

Shiny will only apply one bonus for an item. Their effects are as follows:

| Type | Bonus |
| --- | --- |
| Weapon | +4 Damage (+7 if doublehanded) |
| Stat | +2 Stat |
| Armor | +12 Armor, +10 Resistance |
| Misc | +1 Dex, +1 Int, +1 Str |

[^1]: Using an Ultimate Upgrade Scroll will prevent the item from being lost.
[^2]: [Server code for failing a stat change](https://github.com/kaansoral/adventureland/blob/c584e56f09f2200ffcb53277a9f453a8e41e01bd/node/server.js#L6331).
[^3]: An Essence of Greed is only granted if the item was at least High grade. Common items will not give an Essence of Greed.
[^4]: Not exactly true. See the section on [Karma](#karma).
[^5]: [Effects of the "Lucky Slot" in server code](https://github.com/kaansoral/adventureland/blob/c584e56f09f2200ffcb53277a9f453a8e41e01bd/node/server.js#L6197).
[^6]: 1/1,000,000 chance of success, at the time of writing.
[^7]: [Effect of Prim Stacking in server code](https://github.com/kaansoral/adventureland/blob/c584e56f09f2200ffcb53277a9f453a8e41e01bd/node/server.js#L6087).
[^8]: The TrackTrix is a tricsky fellow, it rounds some numbers when it shouldn't.
[^9]: An example would be the Mech-a Gnome, which drops Electronics.
[^10]: An example of a static global drop would be the PVP token on PVP servers.
[^11]: An example of a normal global drop would be mistletoe during the XMas event.

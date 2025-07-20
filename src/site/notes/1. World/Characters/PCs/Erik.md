---
{"dg-publish":true,"permalink":"/1-world/characters/p-cs/erik/"}
---


>[!cards|no-i no-t  1]
> > [!recite| no-i txt-c] **CAMPAIGN LEVEL**
> > ### `VIEW[{details.campaignLevel}]`

---
# `CHARACTER DETAILS`
> > [!columns| no-i no-t 2]
> > > [!infobox| wfull th ]
|          |         |
| ----------- | ------------- |
| **Name** | `INPUT[text(class(long)):details.characterName]`
| **Clan** | `INPUT[inlineSelect(option(1, Aburame), option(2, Akimichi), option(3, Hatake), option(4, Hyuuga), option(5, Inuzuka), option(6, Nara), option(7, Sarutobi), option(8, Senju), option(9, Uchiha), option(10, Uzumaki), option(11, Yamanaka), option(12, Yuki), option(13, Iburi), option(14, Chinoike), option(15, Kaguya), option(16, Fuma), option(17, Hoshigaki), option(18, Hozuki), option(19, Izuno), option(20, Kamizuru), option(21, Kaaze), option(22, Lee), option(23, Shirogane), option(24, Yotsuki)):clan.name]` |
| **Age** | `INPUT[number(class(very-short)):details.age]` |
| **Gender** |  `INPUT[inlineSelect(option(1, Male), option(2, Female)):details.gender]` |
> >
> > > [!infobox| wfull th ]
|          |         |
| ----------- | ------------- |
| **Rank** | `INPUT[inlineSelect(option(1, Academy Student), option(2, Genin), option(3, Chuunin), option(4, Special Jounin), option(5, ANBU), option(6, Jounin), option(7, Elite Jounin), option(8, Sannin), option(9, Kage)):rank.name]` |
| **Current Village** | `INPUT[inlineSelect(option('Konohagakure no Sato'), option('Sunagakure no Sato'), option('Kirigakure no Sato'), option('Kumogakure no Sato'), option('Iwagakure no Sato'), option('Amegakure no Sato'), option('Otogakure no Sato'), option('Kusagakure no Sato'), option('Takigakure no Sato'), option('Yukigakure no Sato'), option('Uzushiogakure no sato'), option('Yugakure no Sato')):details.currentVillage]` |
| **Original Village** |  `INPUT[inlineSelect(option('Konohagakure no Sato'), option('Sunagakure no Sato'), option('Kirigakure no Sato'), option('Kumogakure no Sato'), option('Iwagakure no Sato'), option('Amegakure no Sato'), option('Otogakure no Sato'), option('Kusagakure no Sato'), option('Takigakure no Sato'), option('Yukigakure no Sato'), option('Uzushiogakure no sato'), option('Yugakure no Sato')):details.originalVillage]` |
| **Alignment** | `INPUT[inlineSelect(option(Lawful Good), option(Lawful Neutral), option(Lawful Evil), option(Neutral Good), option(True Neutral), option(Neutral Evil), option(Chaotic Good), option(Chaotic Neutral), option(Chaotic Evil) ):details.alignment]` |

---

# `ATTRIBUTES`
> [!columns| no-i no-t 6]
> > [!metadata|  bg-c-red no-i txt-c ] STR 
> > ### `VIEW[{attributeScores.str}]`
> 
> > [!metadata|no-i bg-c-blue txt-c] DEX 
> > ### `VIEW[{attributeScores.dex}]`
>
> > [!metadata|no-i bg-c-purple txt-c] INT 
> > ### `VIEW[{attributeScores.int}]`
> 
> > [!metadata|no-i bg-c-pink txt-c] PER 
> > ### `VIEW[{attributeScores.per}]`
> 
> > [!metadata|no-i bg-c-orange txt-c] VIG
> > ### `VIEW[{attributeScores.vig}]`
>
> > [!metadata|no-i bg-c-yellow txt-c] SPI
> > ### `VIEW[{attributeScores.spi}]`

> [!columns| no-i no-t 2]
> > # `COMBAT SKILLS`
> > > [!cards | no-i no-t 4]
> > > > [!recite| no-i] **Close Combat**
> > > > ### `VIEW[{abilityScores.base.mc} + {attributeScores.str}]`
> > > 
> > > > [!recite| no-i] **Ranged Combat**
> > > > ### `VIEW[{abilityScores.base.rc} + {attributeScores.dex}]`
> > > 
> > > > [!recite| no-i] **Dodge**
> > > > ### `VIEW[{abilityScores.base.dodge} + {attributeScores.dex}]`
> > > 
> > > > [!recite| no-i] **Anticipate Movements**
> > > > ### `VIEW[{abilityScores.base.am} + {attributeScores.per}]`
> > > 
> > > 
> > 
> 
> > [!infobox| wfull th]
> > > # `ENERGIES`
> > > > [!metadata|  bg-c-red no-i txt-c ] HP
> > > > ### `VIEW[{combat.currentHP}]` / `VIEW[(10 + ({attributeScores.vig} * 3) + ({details.campaignLevel} * 5))]`
> > > 
> > > > [!metadata|  bg-c-blue no-i txt-c. ] CHAKRA
> > > > ### `VIEW[{combat.currentChakra}]` / `VIEW[(10 + ({attributeScores.spi} * 3))]`

> # `SOCIAL`
> > [!cards | no-i no-t 2]
> > > [!recite| no-i] **Charisma**
> > > ### `VIEW[{abilityScores.social.charisma}]`
> > 
> > > [!recite| no-i] **Manipulation**
> > > ### `VIEW[{abilityScores.social.manipulation}]`
> >
>


# `COMBAT STATS`

> [!columns| no-i no-t 3]
> > [!recite| no-i] **Initiative**
> > ### `VIEW[{skills.Notice.points} + round({attributeScores.per}/2,0) + {skills.Acrobatics.other} + {attributeScores.dex}]`
> 
> > [!recite| no-i] **Dodge Reactions**
> > ### `VIEW[{abilityScores.base.dodge} + {attributeScores.dex} + {attributeScores.dex} + 9]`
> 
> > [!recite| no-i] **Speed**
> > ### `VIEW[round({attributeScores.dex}/2,0) + 10]`m

---

> [!columns| no-i no-t 2] 
> > [!infobox| wfull th]
| Skill            | Total | Points | 1/2 Attr | Other |
| ----------- | ----- | ------ | -------- | ------ |
| Acrobatics | `VIEW[({skills.Acrobatics.points}) + (round({attributeScores.dex}/2,0)) + ({skills.Acrobatics.other})]` | `INPUT[number(class(very-short)):skills.Acrobatics.points]` | `VIEW[round({attributeScores.dex}/2,0)]` DEX | `INPUT[number(class(very-short)):skills.Acrobatics.other]` |
| Arts | `VIEW[({skills.Arts.points}) + (round({attributeScores.int}/2,0)) + ({skills.Arts.other})]` | `INPUT[number(class(very-short)):skills.Arts.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Arts.other]` |
| Athletics | `VIEW[({skills.Athletics.points}) + (round({attributeScores.str}/2,0)) + ({skills.Athletics.other})]` | `INPUT[number(class(very-short)):skills.Athletics.points]` | `VIEW[round({attributeScores.str}/2,0)]` STR | `INPUT[number(class(very-short)):skills.Athletics.other]` |
| Sciences | `VIEW[({skills.Sciences.points}) + (round({attributeScores.int}/2,0)) + ({skills.Sciences.other})]` | `INPUT[number(class(very-short)):skills.Sciences.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Sciences.other]` |
| Focus | `VIEW[({skills.Focus.points}) + (round({attributeScores.int}/2,0)) + ({skills.Focus.other})]` | `INPUT[number(class(very-short)):skills.Focus.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Focus.other]` |
| Culture | `VIEW[({skills.Culture.points}) + (round({attributeScores.int}/2,0)) + ({skills.Culture.other})]` | `INPUT[number(class(very-short)):skills.Culture.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Culture.other]` |
| Disguise | `VIEW[({skills.Disguise.points}) + (round({attributeScores.per}/2,0)) + ({skills.Disguise.other})]` | `INPUT[number(class(very-short)):skills.Disguise.points]` | `VIEW[round({attributeScores.per}/2,0)]` PER | `INPUT[number(class(very-short)):skills.Disguise.other]` |
| Escape | `VIEW[({skills.Escape.points}) + (round({attributeScores.dex}/2,0)) + ({skills.Escape.other})]` | `INPUT[number(class(very-short)):skills.Escape.points]` | `VIEW[round({attributeScores.dex}/2,0)]` DEX | `INPUT[number(class(very-short)):skills.Escape.other]` |
| Stealth | `VIEW[({skills.Stealth.points}) + (round({attributeScores.dex}/2,0)) + ({skills.Stealth.other})]` | `INPUT[number(class(very-short)):skills.Stealth.points]` | `VIEW[round({attributeScores.dex}/2,0)]` DEX | `INPUT[number(class(very-short)):skills.Stealth.other]` |
> >
> 
> > [!infobox| wfull th]
| Skill            | Total | Points | 1/2 Attr | Other |
| ----------- | ----- | ------ | -------- | ------ |
| Animal Handling [x] | `VIEW[({skills.AnimalHandling.points}) + (round({attributeScores.per}/2,0)) + ({skills.AnimalHandling.other})]` | `INPUT[number(class(very-short)):skills.AnimalHandling.points]` | `VIEW[round({attributeScores.per}/2,0)]` PER | `INPUT[number(class(very-short)):skills.AnimalHandling.other]` |
| Mechanisms [x] | `VIEW[({skills.Mechanisms.points}) + (round({attributeScores.int}/2,0)) + ({skills.Mechanisms.other})]` | `INPUT[number(class(very-short)):skills.Mechanisms.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Mechanisms.other]` |
| Medicine [x] | `VIEW[({skills.Medicine.points}) + (round({attributeScores.int}/2,0)) + ({skills.Medicine.other})]` | `INPUT[number(class(very-short)):skills.Medicine.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Medicine.other]` |
| Occultism [x] | `VIEW[({skills.Occultism.points}) + (round({attributeScores.int}/2,0)) + ({skills.Occultism.other})]` | `INPUT[number(class(very-short)):skills.Occultism.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Occultism.other]` |
| Sleight of Hand | `VIEW[({skills.SleightofHand.points}) + (round({attributeScores.dex}/2,0)) + ({skills.SleightofHand.other})]` | `INPUT[number(class(very-short)):skills.SleightofHand.points]` | `VIEW[round({attributeScores.dex}/2,0)]` DEX | `INPUT[number(class(very-short)):skills.SleightofHand.other]` |
| Search | `VIEW[({skills.Search.points}) + (round({attributeScores.per}/2,0)) + ({skills.Search.other})]` | `INPUT[number(class(very-short)):skills.Search.points]` | `VIEW[round({attributeScores.per}/2,0)]` PER | `INPUT[number(class(very-short)):skills.Search.other]` |
| Notice | `VIEW[({skills.Notice.points}) + (round({attributeScores.per}/2,0)) + ({skills.Notice.other})]` | `INPUT[number(class(very-short)):skills.Notice.points]` | `VIEW[round({attributeScores.per}/2,0)]` PER | `INPUT[number(class(very-short)):skills.Notice.other]` |
| Tracking | `VIEW[({skills.Tracking.points}) + (round({attributeScores.per}/2,0)) + ({skills.Tracking.other})]` | `INPUT[number(class(very-short)):skills.Tracking.points]` | `VIEW[round({attributeScores.per}/2,0)]` PER | `INPUT[number(class(very-short)):skills.Tracking.other]` |
| Poisoncraft [x][x] | `VIEW[({skills.Poisoncraft.points}) + (round({attributeScores.int}/2,0)) + ({skills.Poisoncraft.other})]` | `INPUT[number(class(very-short)):skills.Poisoncraft.points]` | `VIEW[round({attributeScores.int}/2,0)]` INT | `INPUT[number(class(very-short)):skills.Poisoncraft.other]` |

---

# `POWERS`
> [!infobox| wfull clean]
> | Power | Level | Effects |
| --- | --- | --- |
|  |  |
|  |  |
|  |  |
|  |  |
|  |  |

<br>

# `FEATS`
> [!infobox| wfull clean]
|       |
| --- | --- | --- |
|  |  |
|  |  |
|  |  |
|  |  |

---

<!-- Level Up -->
```meta-bind-button
label: Level Up!
icon: ""
hidden: true
class: ""
tooltip: LEVEL UP!!!!!!
id: levelUpID
style: primary
actions:
  - type: updateMetadata
    bindTarget: details.totalLevel
    evaluate: true
    value: x + 1

```

<!-- Use Hit Dice -->
```meta-bind-button
label: Use
icon: ""
hidden: true
class: ""
tooltip: "Expend one hit dice."
id: useHDid
style: primary
actions:
  - type: updateMetadata
    bindTarget: combat.hitDiceUSE
    evaluate: true
    value: x + 1

```

<!-- Long Rest -->
```meta-bind-button
label: Long Rest!
icon: ""
hidden: true
class: ""
tooltip: Take a long rest to reset your hit dice and spell slots
id: longRest_id
style: primary
actions:
  - type: updateMetadata
    bindTarget: combat.hitDiceUSE
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: combat.exhaustion
    evaluate: false
    value: "0"
  - type: updateMetadata
    bindTarget: spells.slots1
    evaluate: false
    value: "4"
  - type: updateMetadata
    bindTarget: spells.slots2
    evaluate: false
    value: "3"
  - type: updateMetadata
    bindTarget: spells.slots3
    evaluate: false
    value: "2"

```


<!-- Increase Proficiency Bonus -->
```meta-bind-button
label: "↑"
hidden: true
id: "increment-prof"
class: my-mb-button-down
style: plain
actions:
  - type: updateMetadata
    bindTarget: globalMod.prof
    evaluate: true
    value: x + 1
```

<!-- Decrease Proficiency Bonus -->
```meta-bind-button
label: "↓"
hidden: true
id: "decrement-prof"
class: my-mb-button-down
style: plain
actions:
  - type: updateMetadata
    bindTarget: globalMod.prof
    evaluate: true
    value: x - 1
```

<!-- Increase Speed -->
```meta-bind-button
label: "↑"
hidden: true
id: "increment-speed"
class: my-mb-button-down
style: plain
actions:
  - type: updateMetadata
    bindTarget: globalMod.speed
    evaluate: true
    value: x + 5
```

<!-- Decrease Speed Bonus -->
```meta-bind-button
label: "↓"
hidden: true
id: "decrement-speed"
class: my-mb-button-down
style: plain
actions:
  - type: updateMetadata
    bindTarget: globalMod.speed
    evaluate: true
    value: x - 5
```

<!-- Increase AC -->
```meta-bind-button
label: "↑"
hidden: true
id: "increment-ac"
class: my-mb-button-up
style: plain
actions:
  - type: updateMetadata
    bindTarget: globalMod.ac
    evaluate: true
    value: x + 1
```

<!-- Decrease AC -->
```meta-bind-button
label: "↓"
hidden: true
id: "decrement-ac"
class: my-mb-button-down
style: plain
actions:
  - type: updateMetadata
    bindTarget: globalMod.ac
    evaluate: true
    value: x - 1
```
---
{"dg-publish":true,"permalink":"/2-mechanics/system-rules/check-system/"}
---

The check system governs how a character's actions—such as attacking, tracking, or intimidating—are resolved. Checks use parameters from the character sheet (**attributes**, **skills**, **combat skills**, and **powers**) and typically involve rolling dice, though some situations allow tests without dice. This section outlines the **D8 System** rules for tests.

---

### PRECISION

**Precision** represents a character’s ability to perform an action. It is determined as follows:

- For **skills**, precision equals the skill level (e.g., **Notice 3** means precision 3).
- For **attributes** and **combat abilities** (e.g., Melee Combat (MC), Ranged Combat (RC), Dodge (DOD), Anticipate Movement (AM)), precision is the attribute or ability level.
- For **powers**, use the relevant combat ability’s precision (e.g., **Ranged Combat** for a Katon fireball).

Precision can be modified by **accuracy bonuses** or **penalties** from combat situations, powers, or aptitudes.

---

## TYPES OF CHECKS

The D8 System uses two main test types: **Check Against DC** and **Check Against Check**.

### CHECK AGAINST DC

All checks use **eight-sided dice (d8)**. When “roll 1 die” is mentioned, it refers to **1d8**.

To perform a test:

1. Roll **2d8** and sum the results.
2. Add your **precision** for the relevant attribute, skill, or ability.
3. Compare the total to the test’s **Difficulty Class (DC)**. If equal or higher, you succeed.

**Difficulty  Class (DC)** depends on the target:

- **Against a Target (person/creature that can defend)**: DC = **9 + target’s precision**.
    - Example: Attacking with a kunai uses **2d8 + Ranged Combat**. If the target dodges, DC = **9 + target’s Dodge**.
- **Against a Thing (objects, undefending creatures, situations)**: DC is set by the Game Master, based on skill rules and **campaign level**.

**Campaign Level**: The maximum attribute value allowed in the campaign (e.g., 10 for a level 10 campaign). Difficulties typically range from **6 to 10 above the campaign level** (e.g., 16–20 for level 10). For **combat abilities** (MC, RC, DOD, AM), add **+3** to the difficulty calculation. The Game Master may adjust difficulties as needed.

**Difficulty Table**:

|**Difficulty**|**Task Typically Performed By**|
|---|---|
|Routine (4)|Civilians|
|Very Easy (8)|Genin|
|Easy (12)|Chuunin|
|Medium (16)|Special Jounin|
|Difficult (20)|Jounin|
|Very Difficult (24)|Kage|
|Absurd (28)|Madara|

##### CHECK AGAINST CHECK

When facing active resistance (e.g., attacking vs. blocking [MC vs. MC], hiding vs. searching [Stealth vs. Search]), both parties roll **2d8 + precision**. The higher total wins. If tied, the higher precision wins; if precisions are equal, reroll or the Game Master decides based on the scene.

For non-attack/defense tests, the order of rolling is set by the Game Master.

---

#### AUTOMATIC SUCCESS AND FAILURE

- **Critical Success (15–16)**: Always succeeds, regardless of difficulty. In a **test against test**, a critical success wins unless the opponent also rolls a critical (then reroll).
- **Critical Failure (2–3)**: Always fails, regardless of precision.

In **attack vs. defense** tests:

- The attacker rolls first. A **critical success** negates the defender’s chance to roll.
- A **critical failure** ensures the defender succeeds without rolling.
- A defender’s **automatic success** applies only if the attack wasn’t a critical hit. Defenses like **Dodge** (which don’t require rolls) aren’t affected by automatic success/failure.
- An **automatic success** occurs if the defender uses an invalid defense (e.g., blocking a heavy **Hachimon** attack).

Some maneuvers, techniques, aptitudes, or powers (e.g., **Mercy Strike**) explicitly grant **Automatic Success**, **Automatic Failure**, or **Automatic Critical Hit** under specific conditions.

---

#### NO-DICE TESTS

Tests represent tasks under time pressure or danger. In less demanding situations, dice can be simulated to streamline gameplay. No-dice tests are **not allowed in combat** unless specified.

##### SIMULATE HALF-DIE

If your **precision** is **≥ Difficulty - 4**, assume **1d8 = 4** (simulating half a die) for an automatic success, even under pressure, as the task is trivial. For tests with multiple success levels, assume the minimum success. You may roll for a higher success, or the Game Master may assign a higher level based on circumstances.

##### SIMULATE 1 DIE

Without pressure, assume **1d8 = 8**. This often ensures automatic success for routine tasks but cannot be used in combat or under stress (Game Master’s call). Against **minions**, assume an attack result of **8 + precision**, with the minion defending against it. Roll **2d8** for damage degree.

##### SIMULATE 2 DICE

With unlimited time and no failure penalties, assume **2d8 = 16**. This takes **16 times the normal test duration**. Cannot be used if failure has consequences (e.g., triggering alarms, falling).

---

#### COMPARISON TESTS

When luck isn’t a factor and skill determines the outcome (e.g., arm-wrestling), the character with the **higher attribute/skill level** wins automatically, without rolling (e.g., no “Strength test” needed to compare Strength).

---

#### ACCURACY BONUSES AND PENALTIES

- **Bonuses**: From feats (e.g., **Specialist**, **Reflexes**) or powers (e.g., **Hachimon Tonkou**) apply only to specific tests. For example, **+2 Medicine** for antidotes doesn’t apply to healing tests; **+6 Strength** from Hachimon Tonkou applies to Strength tests and damage but not Melee Combat (MC).
    - Unspecified attack bonuses apply to both **MC** and **RC**; unspecified defense bonuses apply to **DOD**, **AM**, or **MC** (for blocking).
    - Bonuses **exceed campaign level limits** (e.g., Strength 10 + 1 = 11 in a level 10 campaign) but **don’t count toward prerequisites** (e.g., a **+1 CC** from an aptitude doesn’t qualify for **Multiattack**).
    - Multiple bonuses from different sources stack (e.g., **+1 MC** from one aptitude + **+1 MC** from another = **+2 MC**).
- **Penalties**: Apply similarly. If penalties exceed precision, you have **negative precision**. Multiple penalties stack, but only up to **-3** per test.
- **Dodge Bonuses**: Lost if **flat-footed** or unable to move.
- **Size Bonuses**: Permanent **Strength** and **Vigor** bonuses from size count for prerequisites and Hit Points calculations, but temporary size increases (e.g., **Baika no Jutsu**, **Bijuu Form**) do not.
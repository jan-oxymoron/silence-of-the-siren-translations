# What actually needs a translator

Generated 2026-09-16. Of the 770 English strings changed in the last sync:

- 289 are punctuation, quotes, capitalisation, spelling or article fixes: **nothing to do**.
- 331 are rewordings of campaign dialogue, lore and unit/hero descriptions with the same meaning: **nothing to do** unless you want to mirror the new English (CHANGELOG.md has old and new).
- 65 are wording polish of UI and description texts with the same meaning (section B): **optional**.
- 85 change what the text says (section A): numbers, names, mechanics, removed shortcut hints. **These are the ones to act on.**

Verified 2026-09-16 string by string against the current translations in this repo (after the backport from the game): every row below names only the languages whose translation still reflects the old English. Everything else, including all achievement thresholds, the objective counters and the psy ability descriptions, is already correct and is not listed.

Remaining work: RU 28, HU 26, PTBR 26 strings.

## A. Needs a translator

| file | ID | old English | new English | languages | what changed |
|---|---|---|---|---|---|
| CampaignEmpireLVL2.xml | `MESSAGE_CAMPAIGN_EMPIRE_LVL2_START_JOHN_2` | I am afraid you are correct, doctor 8B. Look at this territory. It used to belong to the UNSS before the collapse of space travel, but now, it's sovereign. | I am afraid you are correct, doctor 9B. Look at this territory. It used to belong to the UNSS before the collapse of space travel, but now, it's sovereign. | HU | doctor 8B is now 9B |
| CampaignEmpireLVL4.xml | `MESSAGE_CAMPAIGN_EMPIRE_LVL4_AMPLIFIER_M_5` | Good. We would appreciate your help ... doctor, do you agree? ... Thomas 8B?! | Good. We would appreciate your help ... Doctor, do you agree? ... Thomas 9B?! | RU, HU, PTBR | Thomas 8B is now 9B |
| Empire.xml | `HERO_EMPIRE_7` | Henry Williams 2B | Henry Williams 2A | RU, HU, PTBR | 2B is now 2A |
| Exploration.xml | `CONSUMABLE_RECHARGE_CELL_DIALOG_INFO` | <color=SOTS_COLOR_ENERGY>+20 Energy</color> | <color=SOTS_COLOR_ENERGY>+{1} Energy</color> | RU, HU, PTBR | use the {1} placeholder instead of 20 |
| UI.xml | `EXPLORATION_TOOLTIP_PHASE_DESCRIPTION` | Cycle has 4 phases. All bases generate units at the start of the first phase. | Cycle has {1} phases. All bases generate units at the start of the first phase. | RU, HU | use the {1} placeholder instead of 4 |
| Exploration.xml | `DIALOG_OBJECT_BATTLE_ARENA_TEXT` | Battle three rounds against random armies. <color=SOTS_COLOR_GOLD>Round 1</color> reward: <color=SOTS_COLOR_GOLD>Random resource</color>. <color=SOTS_COLOR_GOLD>Round 2</ | Battle three rounds against random armies. Rewad is based on <color=SOTS_COLOR_RED>hazard</color>. <color=SOTS_COLOR_GOLD>Round 1</color> reward: <color=SOTS_COLOR_GOLD>R | RU, HU, PTBR | reward now depends on hazard; no fixed 25 morale, no fixed +1 attribute |
| Heroes.xml | `SKILL_EFFECT_EXPLORER1` | Permanently adds <color=SOTS_COLOR_MOVEMENT>4 Movement Points</color>.\nMeeting any friendly commander restores <color=SOTS_COLOR_MOVEMENT>2 Movement Points</color> once | Permanently adds <color=SOTS_COLOR_MOVEMENT>8 Movement Points</color>.\nMeeting any friendly commander restores <color=SOTS_COLOR_MOVEMENT>4 Movement Points</color> once | RU, HU, PTBR | numbers |
| Heroes.xml | `SKILL_EFFECT_EXPLORER2` | Permanently adds <color=SOTS_COLOR_MOVEMENT>8 Movement Points</color>.\nMeeting any friendly commander restores <color=SOTS_COLOR_MOVEMENT>4 Movement Points</color> once | Permanently adds <color=SOTS_COLOR_MOVEMENT>12 Movement Points</color>.\nMeeting any friendly commander restores <color=SOTS_COLOR_MOVEMENT>6 Movement Points</color> once | RU, HU, PTBR | numbers |
| Heroes.xml | `SKILL_EFFECT_EXPLORER3` | Permanently adds <color=SOTS_COLOR_MOVEMENT>12 Movement Points</color>.\nMeeting any friendly commander restores <color=SOTS_COLOR_MOVEMENT>6 Movement Points</color> once | Permanently adds <color=SOTS_COLOR_MOVEMENT>16 Movement Points</color>.\nMeeting any friendly commander restores <color=SOTS_COLOR_MOVEMENT>8 Movement Points</color> once | RU, HU, PTBR | numbers |
| InventoryItemsConsumables.xml | `CONSUMABLE_FUEL_STOCK_DESCRIPTION` | Refills <color=SOTS_COLOR_MOVEMENT>15 Movement Points</color> (cannot exceed 100% capacity) | Refills <color=SOTS_COLOR_MOVEMENT>30 Movement Points</color> (cannot exceed 100% capacity) | RU, HU, PTBR | 15 is now 30 |
| InventoryItemsConsumables.xml | `CONSUMABLE_RECHARGE_CELL_DESCRIPTION` | Refills <color=SOTS_COLOR_ENERGY>20 energy points</color> (cannot exceed 100% of capacity). | Refills <color=SOTS_COLOR_ENERGY>25 energy points</color> (cannot exceed 100% of capacity). | RU, HU, PTBR | 20 is now 25 |
| InventoryItemsExplorationArtifacts.xml | `ARTIFACT_VAGRANT_DESCRIPTION` | An artifact.\nAdds <color=SOTS_COLOR_MOVEMENT>10 Movement Points</color> for each turn. | An artifact.\nAdds <color=SOTS_COLOR_MOVEMENT>20 Movement Points</color> for each turn. | RU, HU, PTBR | 10 is now 20 |
| InventoryItemsExplorationEquipment.xml | `EQUIPMENT_FUEL_ADDITIVES_DESCRIPTION` | Adds <color=SOTS_COLOR_MOVEMENT>2 movement points</color>. | Adds <color=SOTS_COLOR_MOVEMENT>4 movement points</color>. | RU, PTBR | 2 is now 4 |
| Patch08PsyAbilities.xml | `ABILITY_HERO_CONFUSION_DESCRIPTION_LVL1` | Reduces initiative and movement of enemy unit stack by 5. | Reduces initiative and movement of enemy unit stack by 40%. | RU, PTBR | 5 is now 40% |
| Patch08PsyAbilities.xml | `ABILITY_HERO_CONFUSION_DESCRIPTION_LVL2` | Reduces initiative and movement of enemy unit stack by 5. Disables melee attacks. | Reduces initiative and movement of enemy unit stack by 40%. Disables melee attacks. | RU, PTBR | 5 is now 40% |
| Patch08PsyAbilities.xml | `ABILITY_HERO_CONFUSION_DESCRIPTION_LVL3` | Reduces initiative and movement of enemy unit stack by 5. Disables melee attacks. Disables ranged attacks. | Reduces initiative and movement of enemy unit stack by 40%. Disables melee attacks. Disables ranged attacks. | RU, PTBR | 5 is now 40% |
| Patch15.xml | `MANUAL_COMBAT_FAR_ATTACK_RANGE` | <color=#FC7EFB>Far Attack</color>\n Range | <color=#FC7EFB>Imprecise Attack</color>\n Range | RU, HU, PTBR | "Far Attack" is now "Imprecise Attack"; use the same term as in your combat UI strings |
| PatchDoomOfEden.xml | `MESSAGE_DOOM_OF_EDEN_ROSI_INTEL` | We've received a message from the secret service – all the raiders have made a non-aggression pact, something along the lines of "first come, first served," which means t | We've received a message from the secret service – all the raiders have made a non-aggression pact, something along the lines of "first come, first served," which means t | RU, HU, PTBR | the old English sentence was broken ("they're only targeting."); it now says "targeting us" |
| Tutorial01.xml | `TUTORIAL_01_WELCOME` | Hi, welcome to a tutorial that will teach you the basics of how to play Silence of the Siren!\nFirst, let's look at the <color=SOTS_COLOR_GOLD>controls</color>. | Hi, welcome to a tutorial that will teach you the basics of how to play Heroes of Science and Fiction!\nFirst, let's look at the <color=SOTS_COLOR_GOLD>controls</color>. | RU | game title is now Heroes of Science and Fiction |
| Tutorial01.xml | `TUTORIAL_01_ATTRIBUTES` | Each commander has <color=SOTS_COLOR_GOLD>three attributes</color>. <color=SOTS_COLOR_GOLD>Exploration efficiency</color> increases your commander's speed by adding movem | Each commander has <color=SOTS_COLOR_GOLD>three attributes</color>. <color=SOTS_COLOR_GOLD>Exploration proficiency</color> increases your commander's speed by adding move | RU, HU, PTBR | attribute is now called "Exploration proficiency"; make it match your translation of the attribute name |
| Pirates.xml | `UNIT_PIRATES_CRAB` | Scorch Sprayer | Scorch Shower | RU, HU, PTBR | unit renamed from Scorch Sprayer to Scorch Shower (keep your own name if it fits) |
| CrusadersBases.xml | `BUILDING_CRUSADERS_DEFENSIVE_MINES` | Mines | Minefield | RU, HU, PTBR | building renamed Mines to Minefield |
| Patch08PsyAbilities.xml | `STACK_STATUS_EFFECT_POLTERGEIST_2` | Poltergeist | Arcane controller | RU, PTBR | status effect renamed to Arcane controller |
| Patch08PsyAbilities.xml | `STACK_STATUS_EFFECT_POLTERGEIST_3` | Poltergeist | Arcane controller | RU, PTBR | status effect renamed to Arcane controller |
| UI.xml | `GAME_EDITOR` | Editor | Map editor | RU, HU, PTBR | Editor is now Map editor |
| Options.xml | `OPTION_MAP_EDITOR_DISABLE_TEXTURE_VARIATION` | Disable texture variation | Disable object randomization | RU, HU, PTBR | option now means object randomization, not texture variation |
| UI.xml | `BUTTON_SKIP` | Pass turn [P] [Space] | Pass turn | HU | remove the shortcut hint |
| UI.xml | `BUTTON_WAIT` | Wait [W] | Wait | HU | remove the shortcut hint |
| UI.xml | `BUTTON_ABILITIES` | Commander's abilities are available!\n(Click on your commander's face)!\n[A] | Commander's abilities are available!\n(Click on your commander's face)! | HU | remove the shortcut hint |
| UI.xml | `TOOLTIP_NEXT_HERO` | Switch to next commander with available actions.\n[N] | Switch to next commander with available actions. | HU | remove the shortcut hint |

## B. Optional (flavor nuance only)

| file | ID | old English | new English | languages | what changed |
|---|---|---|---|---|---|
| PatchDoomOfEden.xml | `MESSAGE_DOOM_OF_EDEN_ROSI_MUSHROOM` | Look, this is a magical mushroom. If you stay near it for a while, it will start to release spores that induce feelings of happiness and joy. Just be careful, we don't ha | Look, this is a magical mushroom. If you stay near it for a while, it will start to release spores that induce feelings of happiness and joy. Just be careful, we don't ha | RU, HU, PTBR | "antidote" became "detox" |
| PatchDoomOfEden.xml | `MESSAGE_DOOM_OF_EDEN_ROSI_TELEPORT_MONEY` | Here's all our available money and other necessary resources. | Here's some our available money and other necessary resources. | RU, HU, PTBR | "all our money" became "some of our money" |
| PatchDoomOfEden.xml | `MESSAGE_DOOM_OF_EDEN_PIRATES` | From now on, let this land be known as the new recreational retreat of the Sovereign Fleet. Objections are not allowed. | From now on, let this land be known as the new region of the Sovereign Fleet. Objections are not allowed. | RU, HU, PTBR | "recreational retreat" became "region" |

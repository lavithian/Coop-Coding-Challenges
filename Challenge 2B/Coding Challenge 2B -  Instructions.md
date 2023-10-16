# **Challenge 2B**

**Please do either _Challenge 2A_ or _Challenge 2B_ but not both (unless you wanna).**

### **To the Wizards of 42 Tower**

Our Majesty has heard of your skills and has requested a battle calculator.

You had been supplied with lists of units for Humans and Orcs.

It;s your job to allocate them appropriate HP and ATK values. Gold should have been allocated for you (tax purposes).

When allocating HP and ATK, keep these in mind:

- [] A single Spearman should be able to handle 2 Goblins before being defeated by the third one.
- [] An Archer has less health than a Spearman.
- [] A single Orc can defeat a Spearman.
- [] A Knight can defeat a Warg.
- [] A warg can defeat 4 archers, after using its Special Ability and ATK.
- [] Pegasus Riders have less HP and ATK than the Knight but higher than the Spearman and Archer together.
- [] It takes two arrows to defeat a Peagus Rider, but only one thrown axe to take it down.
- [] It should take two rounds for a Cleric to fully heal a Spearman.
- [] A grounded Wyvern takes 1.5 more arrows than a Troll to take down.
- [] A Knight should be able to defeat 4 Goblins before receiving damage.
- [] All Ranged Attacks do half of their Melee Attacks, except for Archers. Archers only deal Ranged Attacks.
- [] Clerics can't attack.
- [] Trolls have enough health to withstand 100 arrows. Likewise for a grounded Wyvern.
- [] A Wyvern must come down often enough that a 100 spearman should be able to withstand its fireballs and defeat it.
- [] A troll can defeat 100 Spearmans.
- [] 50 Peguses can down a Wyvern.

#### **Rounds:**

Each round of battles are resolved in the following order:
1. Ranged Attack
2. Damage Received
3. Melee Attack
4. Damage Received
5. Cleric Heals

Special Abilities take effect where relevant.

#### **HP, Health Pools and Unit Count**

1. All units have a Health Pool.

i.e. If a Spearman has (for example) 10HP and there are 100 of them, the total Health Pool of Spearmen is 1000.

2. The unit count is recalculated after receiving damage.

i.e. If Spearmen receives 300 damage, then there are now 70 Spearmen left (700/10).

3. Clerics heal the damage pool, not individual units but cannot heal beyond the maximum Health Pool

i.e. If the Spearmen Health Pool has been weakened to 700HP, then Cleric heals it back to 800HP, then there are now 80 Spearmen left (800/10).

4. A damanged unit has damage penalty when attacking.

i.e. If a Spearman has (for example) 7/10 HP, then it will only do 70% of its original ATK.

#### **Target Priority**

Human Units (except for Pegasus Riders) will target Orc Units in this order:
1. Trolls
2. Goblins
3. Orcs
4. Wargs
5. Wyverns

Pegasus Riders are free to choose what to target every round (the logic provided by you, Sir Wizard).

i.e Humans won't attack Goblins until all of the Trolls have been defeated

Orc Units (except for Wyverns) will target Human Units in this order:
1. Knights
2. Spearmen
3. Clerics
4. Archers
5. Pegasus Riders

Wyverns have a different set of target priorities:
1. Pegasus Riders
2. Archers
3. Knights
4. Spearmen
5. Clerics



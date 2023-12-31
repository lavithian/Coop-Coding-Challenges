# **Challenge 2B**

**Please do either _Challenge 2A_ or _Challenge 2B_ but not both (unless you wanna).**

### **To the Wizards of 42 Tower**

Our Majesty has heard of your skills and has requested a battle calculator.

You had been supplied with lists of units for Humans and Orcs.

It's your job to allocate them appropriate HP and ATK values. Gold should have been allocated for you (for tax purposes).

When allocating HP and ATK, keep these in mind:

- [ ] All HP and (Melee or Ranged) ATK values are whole numbers. No decimal numbers allowed.
- [ ] A single Spearman should be able to handle 2 Goblins before being defeated by the third one.
- [ ] An Archer has less health than a Spearman.
- [ ] A single Orc can defeat a Spearman with a moderate amount of health left.
- [ ] A single Knight can defeat a Warg.
- [ ] A Warg can defeat 4 Archers, after using its Special Ability and ATK.
- [ ] Pegasus Riders have less HP and ATK than a Knight but higher than the sum of Spearman and Archer HP.
- [ ] It takes three arrows to defeat a Peagus Rider, but two thrown axes to take it down.
- [ ] It should take two rounds for a Cleric to fully heal a Spearman.
- [ ] A grounded Wyvern takes 1.5 more arrows than a Troll to take down.
- [ ] A Knight should be able to defeat 4 Goblins before receiving damage.
- [ ] All Ranged Attacks do half of their Melee ATK, except for Archers. Archers only deal Ranged ATK.
- [ ] Clerics can't attack. At all.
- [ ] All Orc units can defeat a Cleric in a single round. All Orc units but Goblins can defeat an Archer in a single round.
- [ ] Trolls have enough health to withstand 100 arrows.
- [ ] A Wyvern must come down often enough that a 100 spearman should be able to withstand its fireballs and defeat it.
- [ ] A Troll can defeat 100 Spearmen.
- [ ] 50 Peguses Riders can down a Wyvern, but barely.

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

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i.e. If a Spearman has (for example) 10 HP and there are 100 Spearmen, the total Health Pool of Spearmen is 1000 HP.

2. The unit count is recalculated after receiving damage.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i.e. If Spearmen receives 300 damage, then there are now 70 Spearmen left (700/10).

3. Clerics heal the Health Pool, not individual units but cannot heal beyond the maximum Health Pool

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i.e. If the Spearmen Health Pool has been weakened to 700HP, then Cleric heals it back to 800HP, then there are now 80 Spearmen left (800/10).

4. A damanged unit has ATK penalty when attacking.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i.e. If a Spearman has (for example) 7/10 HP, then it will only do 70% of its original ATK.

5. Any leftover damage after unit is wiped out is transferred to the units to the next priority.

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;i.e. If Orcs wipeout Knights with 100 ATK leftover, the 100 ATK goes to the next targettable priority (Spearmen).

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
2. Clerics
3. Archers
4. Spearmen
5. Pegasus Riders

Wyverns have a different set of target priorities:
1. Pegasus Riders
2. Archers
3. Knights
4. Spearmen
5. Clerics

#### **Battle Reports**

Your calculator should display turn by turn battle report. It should look something like this:

```
The Battle of 42

Human Army            Orcs Army
Spearmen:       100   Goblins: 100
Archers:        100   Orcs:    100
Clerics:        100   Wargs:   100
Knights:        100   Trolls:  100
Pegasus Riders: 100   Wyverns: 100
Total:          500   Total:   500
----------------------------------
              ROUND 1
----------------------------------

Ranged Attack
Archers shoot and deal X damage to Y units.
Wargs shoot and deal X damage to Y units.
[etc]

Damage Received
Goblins suffered X damage. They lost Y units.
Knights suffered X damage. They lost Y units. Z units turned into Spearmen.

Melee Attack
Goblins deal X damage to Y units.
[etc]

[...]

End of Round Report:
Human Army            Orcs Army
Spearmen:       50   Goblins: 50
Archers:        100  Orcs:    70
Clerics:        100  Wargs:   90
Knights:        70   Trolls:  100
Pegasus Riders: 70   Wyverns: 100
Total:          390  Total:   4100

----------------------------------
              ROUND 2
----------------------------------

[Rinse and Repeat]

```

**Defeat the following compositions**:

(_Try to spend as little gold as possible. We don't want to waste our taxes, do we?_)

&nbsp;&nbsp;&nbsp;&nbsp;300 Orcs

&nbsp;&nbsp;&nbsp;&nbsp;100 Goblins, 500 Orcs

&nbsp;&nbsp;&nbsp;&nbsp;300 Goblins, 300 Orcs, 50 Wargs, 5 Trolls, 1 Wyvern

&nbsp;&nbsp;&nbsp;&nbsp;500 Goblins, 500 Orcs, 100 Wargs, 10 Trolls, 3 Wyverns

&nbsp;&nbsp;&nbsp;&nbsp;1000 Goblins, 1000 Orcs, 200 Wargs, 50 Trolls, 10 Wyverns

&nbsp;&nbsp;&nbsp;&nbsp;1000 Trolls, 1000 Wyverns

&nbsp;&nbsp;&nbsp;&nbsp;10000 Goblins, 5000 Orcs, 1000 Wargs, 100 Trolls, 20 Wyverns

**What's the best composition with this amount of Gold?**

&nbsp;&nbsp;&nbsp;&nbsp;10,000 Gold

&nbsp;&nbsp;&nbsp;&nbsp;100,000 Gold

&nbsp;&nbsp;&nbsp;&nbsp;1,000,000 Gold

&nbsp;&nbsp;&nbsp;&nbsp;1,000,000,000 Gold

&nbsp;&nbsp;&nbsp;&nbsp;9,999,999,900 Gold

**Now fight other teams with your composition!**

(_Don't forget to standardise HP and ATK!!!_)

# CN Dalao Analysis of SVCh
Original source: https://www.bilibili.com/read/cv9421903
Translated by xVarz#8404, please contact with questions or comments.

TL notes:
- the original author and the simulator use phone numpad convention for tile formations; this translation uses keyboard numpad convention for tile formations.

# Overview
Rating: General Use - A+ ~ S, dependent on multiple factors

How to use: conventional general-use offensive RF

Most effective against low HP, high EVA, many-link enemies.

Appreciates RoF buffs.

Satisfactory, can be raised.

# Details
**Candy Echo** - passive: when switching targets, buffs own DMG by 10% for 5 seconds, stacks up to 4 times.

**Candy Echo** - active: for 5 seconds after activating the skill, adds 150 fixed damage\* to each attack that ignores armor, bypasses accuracy checks, bypasses HP shields, and cannot crit; the fixed damage is affected when attacking enemies with multiple links.

\* fixed damage is affected by damage amplification, damage reduction, fixed damage taken (see below), force shields

Note that despite bypassing HP shields, the fixed damage is still affected by the Orthus shield state, which reduces all incoming damage to 1.
![A gif showing SVCh's fixed damage bypassing Orthus shields but only dealing 1 damage.](https://i0.hdslb.com/bfs/article/57d88687b9686fbaeea2bc2860d6aa1fd0481378.gif "SVCh is not a viable Orthus killer.")

# DPS Performance\*
\* Each attack has $\pm$ 15% damage variance, the results below are averaged over 100 simulations. Excluding situations with critical armor values or super high evasion, damage variance does not affect the conclusions below.

For conventional battles using this conventional formation, SVCh's DPS output will vary significantly under different enemy formations and stats:

## Evasion test
When enemies are max linked and with 1 passive stack, between 0 eva and 62 eva, SVCh performs at **0.88-0.92 wa**; under these conditions, she doesn't quite reach T0 RF DPS.

Simulation conditions: WA2000 on 7, Grizzly on 4, SVCh on 1, Calico MOD3 on 5, P22 on 2; Parachute fairy with DMG2 talent, fairy skill off, walk time 0s, battle length 20s, normal enemies, 5 enemy links, 1 enemy group; 0 eva on the left, 62 eva on the right.
![An image showing the formation and the results of the two conditions. On the left, WA2000 deals 188,132 dmg and SVCh deals 166,465 dmg; on the right, WA2000 deals 140,429 dmg and SVCh deals 129,906 dmg.](https://i0.hdslb.com/bfs/article/82309ee69fae70ca9d0c17fe904972515bf412a1.png@1320w_436h.webp)

Enemy EVA has a small effect on SVCh's performance. In practice, when fighting against super-high EVA enemies (e.g. Patrollers), her performance is far weaker than sure-hit RFs.

## Link test
When enemies have 30 EVA and with 1 passive stack, between 0 links and 5 links, SVCh performs at **0.84-0.91 wa**; under these conditions, she still doesn't reach T0 RF DPS.

Simulation conditions: WA2000 on 7, Grizzly on 4, SVCh on 1, Calico MOD3 on 5, P22 on 2; Parachute fairy with DMG2 talent, fairy skill off, walk time 0s, battle length 20s, normal enemies, 30 enemy EVA, 1 enemy group; 1x linked enemies on the left, 5x linked enemies on the right.
![An image showing the formation and the results of the two conditions. On the left, WA2000 deals 165,676 dmg and SVCh deals 138,871 dmg; on the right, WA2000 deals 162,399 dmg and SVCh deals 147,493 dmg.](https://i0.hdslb.com/bfs/article/5dde5be548874166eac819d7e478cc30db63c074.png@1320w_432h.webp)


The number of enemy links has a moderate impact on SVCh's performance. She is not suitable for fighting single-link enemies.

## Enemy kill rate test
When enemies are max linked and have 30 EVA, between killing an enemy every 5s (i.e. consistently 1 passive stack) and every 1.25s (i.e. consistently 4 passive stacks), SVCh performs at **0.91-1.14 wa**; under these conditions, her DPS fluctuates around the T0 RF DPS level.

Simulation conditions: WA2000 on 7, Grizzly on 4, SVCh on 1, Calico MOD3 on 5, P22 on 2; Parachute fairy with DMG2 talent, fairy skill off, walk time 0s, battle length 20s, normal enemies, 5 enemy links, 30 enemy EVA, 1 enemy group; 1 passive stack on the left, 4 passive stacks on the right.
![An image showing the formation and the results of the two conditions. On the left, WA2000 deals 162,399 dmg and SVCh deals 147,493 dmg; on the right, WA2000 deals 165,748 dmg and SVCh deals 188,745 dmg.](https://i0.hdslb.com/bfs/article/23d1f883f024c76b042e6228c98ca58123c2b1aa.png@1320w_432h.webp)

Under ideal conditions (high EVA, high enemy kill rate, max links), SVCh DPS is about **1.21 wa**. In actual combat testing, SVCh DPS fluctuates around **1.0 wa**.

In summary, SVCh is at the edge of T0 RF performance, and the following conditions help her DPS output:
- Low HP enemies, so that enemies die quickly and she quickly switches targets
- High EVA enemies, to make the most of her skill
- Max link enemies, to make the most of her skills
- Pure FP RF echelons, to make the most of ROF buffers

# Team Formation Recommendations
It is recommended to pair her with generalist FP RFs, with SVCh on position 1:
![An image showing an example formation. Lee-Enfield on 7, Five-seveN on 4, SVCh on 1, Px4 Storm on 8, Calico MOD3 on 5.](https://i0.hdslb.com/bfs/article/7c999573d9cc9d39a2e1b8c86ab6b930dc65c923.png@766w_768h.webp)

# Similar Dolls
Higher ranked: N/A

SVCh. Tags are "DPS", "backline", "pos 1", "FP self-buffer", "armor piercing", "fixed damage".

Lower ranked: G28. Tags are "DPS", "backline", "FP self-buffer", "armor piercing".

Similar ranking: Lee-Enfield. Tags are "DPS", "backline", "FP self-buffer", "armor piercing".

# Summary
**Do**: use against hordes, pile RoF buffs, abuse weak mobs

**Don't**: use against single targets, stack FP buffs

**Satisfactory, can be trained**
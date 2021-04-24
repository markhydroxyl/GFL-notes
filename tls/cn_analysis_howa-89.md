# CN Dalao Analysis of Howa Type 89
Original source: https://www.bilibili.com/read/cv4614480

Original author: [命运の乐章](https://space.bilibili.com/8453668)

Translated by xVarz#8404, please contact with questions or comments.

TL notes:
- the original author and the simulator use phone numpad convention for tile formations; this translation uses keyboard numpad convention for tile formations.

# Overview
Rating: General Use - **S**, Specialized Use **S+**

How to use: strong base stats and skill self-buffs

Not bad for typical fights, excels at long fights, manual skill gives 11% better overall DPS

**Must raise**

# Details
**Exam Preparation** - passives: Howa 89 has two attack modes, Revision Mode (default) and Full Marks Mode.
- *Revision*: each shot gives +1 stack of Focus. Upon reaching 18 stacks of Focus, automatically switch to Full Marks Mode.
- *Full Marks*: each shot uses -1 stack of Focus. Each shot in Full Marks mode aims at the enemy with the highest HP, and each consecutive shot on the same target increases Howa 89's damage by 10%, up to 3 stacks. Upon depleting all 18 stacks of Focus, automatically switch to Revision Mode.

**Exam Preparation** - actives: ICD 3s, CD 4s. The effect of proccing the active changes according to which mode Howa 89 is in.
- *Revision*: uses -6 stacks of Focus, will not go negative, can be proc'd at less than 6 stacks of Focus. Buffs FP and RoF by 30% for 4s.
- *Full Marks*: Buffs FP by 30%, and RoF and Acc by 60%, for 6s. Also debuffs self with damage amplification and movement speed reduction by 30%.

# Skill Analysis
While the skill description is very dense and cumbersome, we can immediately see the following:
- in Full Marks Mode, Howa 89 overcaps her own RoF (to 126 RoF).
- the duration of the Full Marks active is not enough time to deplete all 18 stacks of Focus. In the 6s window, only 15 stacks are used. (180/12 = 15)
- in Revision Mode, without any other RoF buffs, proc'ing the active uses 6 stacks of Focus, while Howa 89 gains 8 stacks during the active duration, for a net gain of 2 stacks.

From these observations, we can conclude that:
- Howa 89 barely benefits from RoF buffs.
- in Full Marks Mode, we can maximize DPS increase by waiting for the active buff to end before proc'ing again.
- while in Revision Mode, proc'ing the active delays the start of Full Marks Mode, but an immediate DPS buff is gained. Notice that the two active cycles of only proc'ing the active in Full Marks Mode and proc'ing the active as often as possible (i.e. auto skill) only give localized DPS optimizations. A tradeoff between these two cycles is needed to maximize global DPS.

After some research, the following active cycle (henceforth, manual skill) was found to give the highest overall DPS:
- during Revision Mode, proc the active ASAP (proc #1)
- at the start of Full Marks Mode, proc the active (proc #2)
- immediately after the second proc wears off (i.e. when Howa 89 has 3 stacks left), proc the active again (proc #3)

Theoretical calculations show that, for a typical formation in a typical battle (15 enemy EVA), auto skill (position 1 below) has an advantage earlier (between 7-12.5s),while, at later times, manual skill catches up. In long fights, manual skill gives an **11% DPS increase** over auto skill.

The typical formation is Grizzly on position 4, UMP45 MOD 3 on position 5, P22 on position 2, and the two ARs on positions 1 and 7. Fairy is a 5\* Parachute fairy with DMG 2 talent (reminder that the picture uses phone numpad convention).

![A diagram showing the echelon formation and DPS graph.](https://i0.hdslb.com/bfs/article/75b7889b1eb6774f2b90835216a28d00d7ec2210.png@1320w_380h.webp)

To summarize, auto skill is better for typical fights, while manual skill is better for longer fights.

# DPS Performance
Tests were conducted using the following formation: Grizzly on position 9, UMP45 MOD 3 on position 5, P22 on position 2, and 3 ARs on positions 1, 4, and 7. To demonstrate the practical difference between auto skill and manual skill, the position 7 Howa 89 is in manual skill mode, the position 4 Howa 89 is in auto skill mode, and the position 1 Homete is used as a baseline reference. It is impossible to get proper tile coverage from all three buffers on all three dolls, so Grizzly (originally in position 4) is moved to the corner where her tiles touch none of the ARs, while she is still in the echelon, so she can continue providing FP buffs from her skill; note that this does not affect the relative performance of the three ARs, and so does not affect the conclusions drawn below.

![An image of the formation.](https://i0.hdslb.com/bfs/article/8c4e4704f40f6b936d50f4be86e286f91f9c52d2.png@770w_778h.webp)

**Typical battle** (20s, 15 enemy EVA): Howa 89 performs at **1.23/1.48** Hometes (auto/manual). As enemy EVA increases to 62, Howa 89's ACC self-buff becomes more apparent, causing her DPS to reach **1.24/1.62** Hometes. Notice that Howa 89's dominance is only obvious after 10s, and her performance is practically the same as Homete's in the short-term.

![An image showing the typical battle DPS graph.](https://i0.hdslb.com/bfs/article/17d45d86babca15aec4c185a78b4754e02b3d4c3.png@1320w_456h.webp)
> 15 eva typical fight

**Long battle** (50s): Howa 89 performs at **1.41/1.64** Hometes. As enemy EVA increases to 62, Howa 89's DPS reaches **1.45/1.82** Hometes.

![An image showing the long battle DPS graph.](https://i0.hdslb.com/bfs/article/4fb9703f19e71dae2ae3e1379eacd60daedfd650.png@1320w_456h.webp)
> 15 eva long fight

For comparison, under identical conditions, her DPS is able to *catch up to ST AR-15's* (and exceeds ST AR-15's for even longer fights).

![An image showing the comparison with ST AR-15.](https://i0.hdslb.com/bfs/article/a3fcf015d4807668c597bf2a04935ef721555da9.png@1320w_456h.webp)
> 15 eva comparison with ST AR-15

Empirical evidence (taken from Polarized Light's 100k CE Executioner fight) also shows that her DPS is practically tied with ST AR-15's. Thanks to [白金_世界](https://space.bilibili.com/40599528/) for the empirical test.

![An image showing the DPS chart for the aforementioned fight, where ST AR-15 has dealt 46.0% of the damage while Howa Type 89 has dealt 45.6%.](https://i0.hdslb.com/bfs/article/93a7f3157926a5494042cae5697277ce062fd1d5.png@1320w_610h.webp)

However, remember that adding M4A1 MOD will put ST AR-15 back in the lead, and there's no way for Howa 89 to match ST AR-15's night dominance.

![An image of a ST AR-15 chibi repeatedly saying "M4M4M4M4..."](https://i0.hdslb.com/bfs/article/3195abc466539f3d9d87a15e127b2879e8592426.gif)
> M4M4M4M4M4M4M4M4M4M4M4

# Team Recommendations
Put her in any random ARSMG team that doesn't have many RoF buffs. A bit of RoF will have a minor impact on Howa 89's performance.
![An image showing two possible formations including Howa 89. The first has Howa 89, Grizzly, AK-12, UMP45 MOD, and P22. The second has Howa 89, Grizzly, ST AR-15, Dorothy, and P22.](https://i0.hdslb.com/bfs/article/9454824a6399532ae187ea217e084e0e911e5981.png@1320w_828h.webp)

# Summary
**Good for general use, excels at long fights, manual skill for top performance**

**MUST RAISE**

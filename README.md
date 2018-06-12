Fatherhood mod

This mod adds proximity to adult males as a scalar for birth probability.
This means that being near an adult male makes you more likely to have a baby and
being far away from adult males means you are less likely
It also adds Adam, who spawns next to an Eve so that she is not disadvantaged by
being far away from men. Every Eve will have one Adam.

It also refactors the lineage system to track father and mother relationship separately.
If another player is related to the current player through both their mother and their father,
the closest of the two relationships will be the one shown.

There are two variables defined in the server/settings folder:

fatherMinDistance: (default 10) all adult males within this proximity of a potential mother have the same
chance of being the father of the baby and being closer than this distance does not increase the chances
of having a baby.

fatherMaxDistance: (default 49) the distance beyond which all adult males are given the same minimum probability
of being the father of the baby and being further than this distance does not decrease the chances of having
a baby.

The probability of having a baby is scaled between the minimum and maximum distance values. If there
are no adult males on the server, then the next player will spawn as an Eve.
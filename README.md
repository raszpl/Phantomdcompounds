# Phantom Doctrine Body Engineering compounds visual assistant

Directly reachable at https://raszpl.github.io/Phantomdcompounds/compounds.html

This visual assistant will let you decide which compound order is best at particular game chapter. For example the best possible one [139,126,130,103,498] is only optimal after reaching chapter 7, but [149,109,130,91,479] is stronger from chapter '3 Part 2' all the way to '7 part 1'. In chapter 5 difference is quite dramatic between the two, "optimal" one boosting only 159, while "inferior" series giving 323 additional points. This results in huge Damage Threshold and Movement Range bonuses in mid game.


I hardcoded 30 best Compound series from http://phantom-doctrine.wikia.com/wiki/Body_Engineering . Re sorting allowed discovery of some duplicates/naive series, for example best respiratory [122,99,140,82,443] and [97,75,140,90,402] series are pretty much the same, with later missing one component.


I had to manually reverse engineer correlations between main four stats and their derivatives. There are some curious quirks. Movement Range is directly tied to Respiratory and jumps up at 68, 98, and 130 tresholds, BUT it appears to drop back to 5 when Max Action Points reaches 3. I need more datapoints (higher level agent stats) to research it further. Movement Range calculation should be considered broken at this stage.

# Help
- Select progress (slider) or Chapter (drop down menu). This will show available compounds at particular point in the game. Black = available.
- Manually clicking on compounds enables/disables ones you have/are missing.
- Reaching  chapter '4 Part 1' in the game unlocks "Remove All" Body Engineering option. This lets you see Agents raw stats. Entering those enables chosing best possible compound series for particular agent.
- "Preview" button switches between calculating whole series vs calculating only currently unlocked compounds in the series.
- "Sort" button switches between original series from wikia vs properly sorted according to game unlock order.
- Hovering over main stats (Circulatory/Sensory/Respiratory/Motoric) will highlight in yellow directly dependent parameters.
- Hovering over compound visualizes compounds it requires (green) and blocks (red). Both should be always on the left side of every compound for the series to be valid.


# todo
- Finish reverse engineeing stats>attribute correlation, fix Movement Range.
- Add perks influencing stats.
- Maybe work on color selection ;)


# Used resources
- http://phantom-doctrine.wikia.com/wiki/Body_Engineering
- http://phantom-doctrine.wikia.com/wiki/Technology_Tree
- http://phantom-doctrine.wikia.com/wiki/Agents
- https://www.reddit.com/r/PhantomDoctrine/comments/98cp8x/psa_perks_and_abilities_what_they_do_numbers/
- https://docs.google.com/spreadsheets/d/1aNCZELoeWJ6CJuOg2ZVG7a0x7XilbewP4RsXT3NZvb8
- https://steamcommunity.com/sharedfiles/filedetails/?id=1489919688

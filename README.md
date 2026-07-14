Platinum Kaizo — Gen 4 Switch-In Calculator

A browser-based tool that predicts which Pokémon a Platinum Kaizo trainer will send in next, based on the real Gen 4 trainer AI logic (type-matchup scoring, supereffective move checks, and damage-based fallback).

Open the calculator — no download or install needed, just open the link.

What it does


Search any of the 483 trainers in the game by name and auto-load their exact team (species, level, stats, abilities, items, and movesets), pulled from verified community data.
Search any of the 505 species in the game to auto-fill your own active Pokémon's type.
Predicts the opponent's next Pokémon using the same three-phase logic the real game uses:

Phase 1 (type): sorts the opposing party by type-matchup score, then finds the first one with an actual supereffective move against you.
Phase 2 (damage): if no one qualifies, calculates real damage output for every move on every Pokémon and picks whoever hits hardest.
Phase 3 (fallback): if nothing can land a hit, defaults to whoever's first in the party.



Handles ability-based immunities (Levitate, Volt Absorb, Water Absorb, Flash Fire, Wonder Guard, etc.) on your active Pokémon.
Supports double battles — including the game's actual double-battle trainer pairings, which are detected and merged automatically when you load either trainer's name.


How to use it


Search for your active Pokémon's species (or set its type manually), and fill in its real Defense/Special Defense — accuracy here matters a lot, since two Pokémon with the same typing can have very different Def/SpD splits.
Search for the trainer you're fighting, or add opponent Pokémon manually.
Hit Calculate to see who's most likely to be sent in next, and why.


Known limitations


Damage calculations don't model crits, random rolls, items, weather, or a handful of nonstandard moves (Counter, Endeavor, etc.) — this is a planning tool, not a frame-perfect simulator.
The opponent's actual send-in order after their lead can shift based on your team, since the real AI reacts dynamically — treat predictions as "the right call whenever this Pokémon appears," not a guaranteed script.
Trainer and move data reflect the game's state as of when this was built. If Platinum Kaizo receives balance changes, this won't auto-update.


Credits

Trainer, species, and move data cross-referenced from the Platinum Kaizo community's own open-source calculator project and the Gen IV trainer AI documentation.

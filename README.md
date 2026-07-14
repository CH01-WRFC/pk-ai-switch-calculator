Platinum Kaizo — Gen 4 Switch-In Calculator

A browser-based tool that predicts which Pokémon a Platinum Kaizo trainer will send in next, based on the real Gen 4 trainer AI logic — verified line-by-line against the documented switching AI and move-selection AI mechanics, not just type-chart intuition.

Open the calculator — no download or install needed, just open the link.

What it does


Search any of the 483 trainers in the game by name and auto-load their exact team (species, level, stats, abilities, items, and movesets), pulled from verified community data.
Search any of the 505 species in the game to auto-fill your own active Pokémon's type.
Import your own team by pasting it in the standard export format (nickname, species, ability, level, nature, IVs, moves) — it parses your whole team, computes real stats, and lets you drop any of them straight into the active-Pokémon fields with one click.
Predicts the opponent's next Pokémon using the same three-phase logic the real game uses:

Phase 1 (type): sorts the opposing party by type-matchup score, then finds the first one with an actual supereffective move against you.
Phase 2 (damage): if no one qualifies, calculates real damage output for every eligible move on every Pokémon and picks whoever hits hardest.
Phase 3 (fallback): if nothing can land a hit, defaults to whoever's first in the party.



Doubles support, including the game's actual double-battle trainer pairings (detected and merged automatically) and trainers who send out two of their own Pokémon at once.


Mechanics modeled (all confirmed against the documented Gen 4 trainer AI rules)


Held items on opponent Pokémon: Choice Band/Specs, type-boosting items (Charcoal, Mystic Water, etc.), species-locked items (Light Ball, Thick Club).
Weather (Sun/Rain boosting or weakening Fire/Water moves) and Gravity (grounds Flying-types and Levitate holders).
Light Screen / Reflect (halves incoming Special/Physical damage for the side they're set on).
Target-side immunity and resist abilities: Levitate, Volt Absorb, Water Absorb, Flash Fire, Sap Sipper, Storm Drain, Lightning Rod, Wonder Guard, Thick Fat, plus Iron Ball as a held item.
Opponent-side abilities: Huge Power/Pure Power (doubled Attack), Adaptability (2x STAB), Normalize (all moves count as Normal-type), Scrappy (Normal/Fighting bypasses Ghost immunity), Mold Breaker (ignores all target immunity abilities).
The documented dual non-immunity glitch — a real Gen 4 bug where a dual-type Pokémon whose first-listed type is immune to a move, but whose second type is weak to it, gets incorrectly flagged as hit supereffectively anyway.
The documented 255-damage overflow bug and 320-score overflow bug in the AI's own calculations.
The documented list of moves the AI's damage check ignores entirely (Explosion, Self-Destruct, Focus Punch, Hyper Beam, Frenzy Plant, and about a dozen others) — even though they deal real damage in an actual fight, the AI's own decision-making treats them as dealing none.


Deliberately NOT modeled, because the documented AI itself ignores these for this specific check: Life Orb, Metronome, Expert Belt, Tinted Lens, Filter/Solid Rock, critical hits, and random damage variance.

How to use it


Search for your active Pokémon's species (or import your team, or set its type manually), and fill in its real Defense/Special Defense — accuracy here matters a lot, since two Pokémon with the same typing can have very different Def/SpD splits.
Search for the trainer you're fighting, or add opponent Pokémon manually.
Set weather, Gravity, or Light Screen/Reflect if any are active in the fight.
Hit Calculate to see who's most likely to be sent in next, and why.


Known limitations


This models who gets sent in after a KO — it does not model the separate mid-battle mechanic of a trainer voluntarily withdrawing an already-active Pokémon (e.g., for a bad type matchup, a status condition, or an absorb ability), which follows different, more complex rules.
Abilities that trigger below 1/3 HP (Torrent, Blaze, Overgrow, Swarm) aren't modeled, since the tool has no way to track current HP.
Critical hits, random damage variance, and a small number of nonstandard/fixed-damage moves (Counter, Endeavor, etc.) aren't modeled — this is a planning tool, not a frame-perfect simulator.
The opponent's actual send-in order after their lead can shift based on your team, since the real AI reacts dynamically — treat predictions as "the right call whenever this Pokémon appears," not a guaranteed script.
Trainer and move data reflect the game's state as of when this was built. If Platinum Kaizo receives balance changes, this won't auto-update.
This is built from community-documented reverse engineering of the Gen 4 AI, not the original source code — there may be edge cases the documentation itself doesn't cover.


Credits

Trainer, species, and move data cross-referenced from the Platinum Kaizo community's own open-source calculator project. AI mechanics verified against the Gen IV trainer AI move-selection and switching AI documentation.

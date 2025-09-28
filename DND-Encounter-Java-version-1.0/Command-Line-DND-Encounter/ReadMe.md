D&D Encounter Generator (Command Line)

This is a command-line Java application that generates randomized encounters for Dungeons & Dragons (or other tabletop RPGs). It provides monsters, NPCs, items, buildings, species, and even wild magic effects across a variety of environments such as forests, tundras, deserts, towns, and more.

Features

Random Encounters by Environment
Forest, tundra, desert, mountain, underground, grasslands, hamlets, towns, cities, and ports each have unique enemy tables.

Example: A forest encounter might spawn a Bandit, Treant, or Forest Guardian depending on the challenge rating.

Challenge Rating (CR) Scaling
Encounters are generated with CRs ranging from 0.25 to 10.0, chosen randomly to match the adventure difficulty.

Wild Magic Surges
Over 100 possible wild magic outcomes, from minor inconveniences (your armor falls off) to game-altering events (you polymorph into a Paraceratherium).

Items, Buildings, and People
Randomized utility tables allow quick generation of loot, NPCs, and urban structures.

Species Generator
Randomized races for NPCs, from common (Human, Dwarf, Elf) to rare (Ratatosk, Dragonborn, Felidarian).

How It Works

Run the program in your terminal:

java org.peterjordahl.App


You’ll be prompted for:

Party Size (number of adventurers)

Total Party Level (sum of all levels)

Based on these inputs, the generator will:

Select a random environment table.

Roll a random Challenge Rating.

Output a suitable enemy encounter.

After the encounter, you’ll be asked:

Do you need another encounter? (YES) or (NO)


Typing YES rolls a new encounter.

Typing NO exits with a friendly message.

Example Run
How many adventurers are in your party? 4
What is the total of all of their levels? 12

>> Encounter Generated: A CR 4.0 Ice Elemental emerges from the tundra!

Do you need another encounter? (YES) or (NO) YES
Exciting!

>> Encounter Generated: A CR 0.5 Smuggler lurking in the port!

Project Structure

Maps of Encounters: Each biome or settlement type maps CRs to monsters.

Utility Generators: Randomized wild magic, items, buildings, NPCs, and species.

Scanner Input: Accepts user choices for repeat encounters.

Requirements

Java 17+ (or compatible JDK)

Command-line execution environment

Future Enhancements

Add difficulty scaling based on average party level.

Support saving encounters to a session log.

Expand monster, magic, and item tables.

Optional “environment selection” instead of purely random rolls.
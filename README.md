A command-line Java application that generates randomized encounters for Dungeons & Dragons (or other tabletop RPGs).
The generator creates monsters, NPCs, items, buildings, species, and even wild magic effects across multiple environments such as forests, tundras, deserts, towns, and ports.

✦ Features

Random Encounters by Environment
Each environment (forest, tundra, desert, mountain, underground, grasslands, hamlets, towns, cities, ports) has its own encounter table.

Example:

Forest → Bandit, Treant, Forest Guardian

Port → Smuggler, Pirate Captain, Kraken Spawn

Challenge Rating (CR) Scaling
Encounters are generated with CR values from 0.25 to 10.0, chosen randomly for varied difficulty.

Wild Magic Surges
Over 100 possible wild magic effects, from silly (your armor falls off) to catastrophic (you polymorph into a Paraceratherium).

Loot, Buildings, and NPCs
Utility tables generate random items, structures, and townsfolk on demand.

Species Generator
Randomizes fantasy races:

Common → Human, Dwarf, Elf

Uncommon → Dragonborn, Felidarian, Ratatosk

✦ How It Works

Run the program in your terminal:

java org.peterjordahl.App


Enter your party size and total party level when prompted.

The generator will:

Select a random environment

Roll a random CR

Output a suitable encounter

After each result, you’ll see:

Do you need another encounter? (YES) or (NO)


Type YES → rolls a new encounter

Type NO → exits with a friendly farewell

✦ Example Run
How many adventurers are in your party? 4
What is the total of all of their levels? 12

>> Encounter Generated: A CR 4.0 Ice Elemental emerges from the tundra!

Do you need another encounter? (YES) or (NO) YES
Exciting!

>> Encounter Generated: A CR 0.5 Smuggler lurking in the port!

✦ Project Structure

Encounter Tables
Environment → Challenge Rating → Monster/NPC

Utility Generators
Wild magic, items, buildings, NPCs, species

User Input
Powered by Scanner, loops until player exits

✦ Requirements

Java 17+ (or compatible JDK)

Command-line environment

✦ Future Enhancements

Difficulty scaling based on average party level

Optional environment selection instead of pure randomness

Expanded monster, item, and magic surge tables

Save encounters to a session log file

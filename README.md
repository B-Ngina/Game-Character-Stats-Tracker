# Game-Character-Stats-Tracker
A robust Python-based class for managing game character statistics, featuring built-in data validation and state management.

This project provides a GameCharacter class that handles core RPG mechanics such as health, mana, and leveling. It is designed to ensure character stats remain within logical boundaries—preventing negative health or mana, and enforcing maximum stat limits—through the use of Python properties.

It's features include:

Data Encapsulation: Uses @property decorators to manage access to character attributes.

Stat Clamping: Automatically limits health and mana values to defined ranges (0–100 for health, 0–50 for mana).

Leveling System: Includes a level_up method that increments the character's level and resets primary resources.

Clean Formatting: Provides a built-in __str__ method for easy status reporting.


Usage Example:

 Initialize a new character
hero = GameCharacter("Adventurer")

 Stats are automatically managed
hero.health = -20  # Automatically sets health to 0
hero.mana = 60     # Automatically sets mana to 50

 Leveling up
hero.level_up()
 Output: #"Adventurer leveled up to 2!"


The GameCharacter class acts as an observer and manager of character data. By utilizing setter methods, the class ensures that any attempt to set health or mana outside of allowed parameters is corrected before the value is stored

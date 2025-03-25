# Turn-Based Battle Game

A simple Python-based turn-based battle game where the player can choose from multiple character classes to battle against an Evil Wizard. The game involves character creation, using special abilities, attacking, healing, and a battle system with randomized attack damage.

## Features
- Choose between four character classes: Warrior, Mage, Archer, and Paladin.
- Each class has unique special abilities.
- The player can attack, heal, or use special abilities during the battle.
- The Evil Wizard regenerates health each turn and attacks the player.
- Victory is achieved when the Evil Wizard's health reaches zero, or defeat occurs if the player's health reaches zero.
- Includes randomized damage for more dynamic gameplay.

## Classes

### 1. **Character**
The base class for all character types. It includes:
- **Attributes**: `name`, `health`, `attack_power`, `max_health`.
- **Methods**:
  - `attack(opponent)`: Deals damage to an opponent with a randomized range based on the character's attack power.
  - `display_stats()`: Displays the character's current health and attack power.
  - `heal()`: Heals the character for a fixed amount, ensuring health doesn't exceed the maximum.

### 2. **Warrior**
The Warrior class inherits from `Character` and has:
- **Power Attack**: A special ability that deals higher damage than a regular attack.

### 3. **Mage**
The Mage class inherits from `Character` and has:
- **Cast Spell**: A powerful spell that deals high damage to the opponent.

### 4. **Archer**
The Archer class inherits from `Character` and has:
- **Quick Shot**: A ranged attack that deals double damage.
- **Evade Attack**: The Archer can avoid the next attack from the opponent.

### 5. **Paladin**
The Paladin class inherits from `Character` and has:
- **Holy Strike**: A special attack that deals bonus damage.
- **Divine Shield**: Blocks the next attack from the opponent.

### 6. **EvilWizard**
The Evil Wizard class also inherits from `Character` and has:
- **Regenerate**: The Evil Wizard regenerates health by a small amount at the beginning of each turn.

## How to Play

### Step 1: Character Creation
- Upon starting the game, you will be prompted to choose your character class from:
  - Warrior
  - Mage
  - Archer
  - Paladin

### Step 2: Battle
- After character creation, you'll enter into a battle with the Evil Wizard.
- In each turn, you can:
  - **Attack**: Perform a regular attack on the Evil Wizard.
  - **Use Special Ability**: Choose from the available special abilities (each class has different abilities).
  - **Heal**: Heal your character to restore health.
  - **View Stats**: Check your current stats, including health and attack power.
  
- The Evil Wizard will regenerate health each turn and attack the player in return.

### Step 3: Victory or Defeat
- The game ends when either the player or the Evil Wizard's health reaches zero.
- If the Evil Wizard is defeated, you win the battle. If your character is defeated, the game ends in defeat.

## How to Run the Game

1. Make sure you have Python 3.x installed.
2. Save the code in a file named `battle_game.py`.
3. Run the game using the following command:

   ```bash
   python battle_game.py
Follow the on-screen instructions to select your character and take actions during the battle.
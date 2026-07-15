# LuckyWheel

A standalone, high-performance Lucky Wheel plugin designed for PocketMine-MP API 5. This plugin allows players to spin a virtual wheel to win custom rewards using either XP levels or Diamonds.

## Features

* **Zero Dependencies:** No external form libraries (like FormAPI) or Composer packages required.
* **Fully Configurable:** Customize costs, reward chances, and execution commands.
* **Dynamic Animations:** Real-time spinning animation with custom title effects and sounds.
* **Modern Codebase:** Built using PHP 8.1+ strict typing and native PocketMine-MP API 5.0.0 standards.

## Installation

1. Drop the `LuckyWheel` folder into your server's `plugins/` directory.
2. Restart your server to generate the default configuration.
3. Edit `resources/config.yml` to set up your rewards.
4. Restart the server or reload plugins.

## Commands & Permissions

| Command | Description | Permission | Default |
| :--- | :--- | :--- | :--- |
| `/luckywheel` | Opens the Lucky Wheel GUI | `luckywheel.use` | `true` |

## Configuration

The plugin generates a clean `config.yml` file. Here is an overview of how the settings look:

```yaml
cost:
  type: "xp"
  amount: 5
rewards:
  - name: "§bDiamond Sword"
    chance: 15
    cmd: "give {player} diamond_sword 1"
  - name: "§e32 Gold Ingots"
    chance: 35
    cmd: "give {player} gold_ingot 32"
  - name: "§c64 Cobblestone"
    chance: 40
    cmd: "give {player} cobblestone 64"
  - name: "§610 Diamond Blocks"
    chance: 10
    cmd: "give {player} diamond_block 10"
# code_project

# Rescue Mission: Every Life Matters
Project Link - https://arcade.makecode.com/S95826-01793-69811-64879

**Rescue Mission: Every Life Matters** is a three-level, 2D animal rescue game created in **Microsoft MakeCode Arcade** for a Creative Coding project. Players explore different environments, collect supplies, treat animals and bring them safely to a rescue centre before their individual rescue deadlines expire.

The game is designed to demonstrate block-based programming concepts such as variables, conditional statements, events, loops, functions, sprites and tilemaps.

## Game objective

Rescue as many animals as possible. Each animal needs **food**, **water** or a **medkit** before it can be carried to the rescue centre. You can carry **one animal at a time**. Avoid hazards, manage your health and resources, and finish all three levels.

## Features

- **Three levels:** Forest Rescue (3 animals), Urban Rescue (4 animals) and Storm Emergency (5 animals).
- **Individual rescue deadlines:** Each animal has its own countdown. An animal disappears if its deadline expires.
- **Resource collection:** Pick up food, water and medkits to treat animals or recover health.
- **Health and hazards:** Start each level with 5 health points; touching a hazard reduces health, with a short protection period between hits.
- **Scoring:** Collecting a supply earns 5 points. Successful deliveries earn 10, 20 or 30 points in Levels 1, 2 and 3 respectively. Missing an animal deducts 10 points, but the score cannot go below zero.
- **Scrolling maps:** The camera follows the player across compact tile-based environments.
- **Level progression:** The game reports how many animals were rescued or missed before proceeding to the next level.

## Controls

| Control | Action |
|---|---|
| Arrow keys / directional controls | Move the player |
| **A** | Cycle through food, water and medkit for healing |
| **B** | Use the selected supply to restore health |
| Touch an animal | See its required supply; treat and pick it up if you have that supply |
| Touch a supply | Collect it automatically |
| Touch the rescue centre while carrying an animal | Deliver the animal automatically |

**Healing:** Food and water each restore 1 health point; a medkit restores up to 2. Health cannot exceed 5. Healing consumes supplies that could otherwise be used for animal rescues.

## Levels

| Level | Setting | Animals | Overall level timer |
|---|---|---:|---:|
| 1 | Forest Rescue | 3 | 150 seconds |
| 2 | Urban Rescue | 4 | 145 seconds |
| 3 | Storm Emergency | 5 | 140 seconds |

Individual animals also have separate rescue deadlines. The level timer and animal deadlines are different mechanics.

## Requirements

- A computer with a modern web browser and access to **[Microsoft MakeCode Arcade](https://arcade.makecode.com/)**.
- **No separate installation, external library or package manager is required** to run the game in the online MakeCode Arcade editor.
- Internet access is needed to open the online editor initially; MakeCode's offline availability depends on how it is set up.

The project uses MakeCode Arcade's built-in APIs for sprites, controllers, scenes, tiles, game information, music and effects. It also uses sprite data functions for animal and supply properties.

## How to run the project

1. Visit **https://arcade.makecode.com/**
4. Open this repository and download arcade-Rescue-Mission.uf2 file.
5. Import it into arcade.makecode. 
6. Switch to **Blocks** to view and edit the game's block-based logic.

## How to play

1. Move around the level to find animals and supplies.
2. Touch an animal to discover whether it needs food, water or a medkit.
3. Collect the required item and return to the animal to treat it.
4. Carry the treated animal to the rescue centre. You cannot carry a second animal until the first has been delivered.
5. Avoid hazards and use **A** and **B** to heal when needed.
6. Rescue animals before their individual deadlines. When all animals have been rescued or missed, the level ends and the next level begins.

## Programming concepts demonstrated

- **Variables:** Track health, score, current level, supplies, rescued animals and missed animals.
- **Conditional statements:** Check resource availability, carrying status, hazard protection and level completion.
- **Events:** Detect sprite overlaps, controller button presses and timed updates.
- **Loops:** Process active animals and update their remaining rescue time.
- **Functions:** Organise level setup, sprite creation, supply distribution and game progression.
- **Random numbers:** Assign animal supply requirements and individual rescue deadlines.
- **Tilemaps and camera:** Build the three environments and keep the player visible as the map scrolls.

## Known limitations and design choices

- Only **one animal can be carried at a time**.
- Animals cannot be rescued without their assigned supply.
- Each animal's deadline continues to decrease while it remains on the map.
- Missed animals disappear and cause a score penalty; the game continues.
- The maps and sprite graphics are intentionally simple to support understanding and editing in MakeCode Arcade Blocks.
- The game is designed for the MakeCode Arcade environment; it is **not a standalone Windows or mobile application**.
- This project has been confirmed to work in the MakeCode Arcade simulator and Blocks editor. It has not been separately verified on physical Arcade hardware.

## Project development

The game began as a simpler fixed-screen rescue prototype. During development, rescue requirements, individual deadlines, healing, hazards and three levels were added. The environments were later redesigned with compact scrolling tilemaps and a player-following camera. Feedback that JavaScript was not the primary classroom programming approach led to ensuring the final project could also be opened and understood in **MakeCode Arcade Blocks**.

## Project files

The repository contain the final MakeCode Arcade source file (`arcade-Rescue-Mission.uf2`) and this `README.md`. 

## Credits and resources

- [Microsoft MakeCode Arcade](https://arcade.makecode.com/) — game development environment.
- [MakeCode Arcade documentation](https://arcade.makecode.com/reference) — reference for built-in programming features.




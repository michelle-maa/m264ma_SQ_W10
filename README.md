# m264ma_SQ_W10

## Updates to Code

Using Week 6's example code, I updated the code to have three meaningful changes: 
- Added a timer. Players must complete the game before 1.5mins. 
- Added star collectables for the player, giving them an accomplishment if they collect all three. 
- Added a start screen that appears before game play state. 

## Setup and Interaction Instructions

To run the sketch locally, open `index.html` in Google Chrome using Live Server.

**Controls:**
- Move: WASD
- Shoot: Spacebar (shoots in the direction you last moved)
- B: Skip to boss fight (testing only)
- Restart: R (after win or game over)
- Start Game: ENTER key 

Explore the world, survive enemy waves as you move north, then enter the glowing boss zone to fight the giant orange blob. Watch the minimap to track enemies off screen.

**Adding Your Own Sounds**
1. Add your sound files to `assets/sounds/`
2. In `preload()`, uncomment the `loadSound()` lines and update the file paths
3. Uncomment the `play()` or `loop()` calls in the relevant functions — there are hooks for the boss music transition too

**Editing the Waves and Boss**
Open `data/enemies.json` to change when waves spawn, how many enemies appear, their speed, and the boss stats. Each wave has a `spawnAt` world Y value — lower values trigger later since the player starts at the bottom of the world.

**Opening the Chrome Console**
- **Windows:** Press `F12` or `Ctrl + Shift + J`, then click the **Console** tab
- **Mac:** Press `Cmd + Option + J`

## Assets

| File                                          | Source                                     |
| ----------------------------------------------| -------------------------------------------|
| `assets'/sounds/bg_music.wav`                 | Sound by MatthewHenry / Freesound [4]      |
| `assets'/sounds/laser_shot.wav`               | Sound by djfroyd / Freesound [2]           |
| `assets'/sounds/player_hurt.flac`             | Sound by Iwan Gabovitch / Freesound [3]    |
| `assets'/sounds/star_twinkle.wav`             | Sound by Robinhood86 / Freesound [5]       |
| `assets'/sounds/win_sound.wav`                | Sound by avreference / Freesound [1]       |

Google Gemini was used to generate the character sprite sheet. 

## References

[1] avreference. 2024. Congrats FX, Freesound. Retrived July 22, 2026 from https://freesound.org/people/avreference/sounds/737181/

[2] djfroyd. 2016. laser one-shot #1.wav, Freesound. Retrived July 22, 2026 from https://freesound.org/people/djfroyd/sounds/348164/

[3] Iwan Gabovitch. 2013. Damage, Freesound. Retrived July 22, 2026 from https://freesound.org/people/qubodup/sounds/211634/

[4] MatthewHenry. 2023. Action Music Loop 2 "Hunted", Freesound. Retrived July 22, 2026 from https://freesound.org/people/MathewHenry/sounds/685597/

[5] Robinhood86. 2025. 13819 star twinkle ding, Freesound. Retrived July 22, 2026 from https://freesound.org/people/Robinhood76/sounds/819418/


# Mod is still in Development!


# Plants vs. Zombies (HTML, CSS, JavaScript)

A lightweight, browser-based implementation of the classic lane defense game, Plants vs. Zombies, built entirely with HTML, CSS, and vanilla JavaScript. No frameworks or external dependencies required — just open in your browser and protect your brains!

## 🌱 Features

*   Classic lane-based tower defense strategy
*   Waves of unique zombies with different abilities 🧟
*   Sun collection and resource management ☀️
*   An arsenal of plants with special powers 💥
*   Responsive design for desktop and mobile 📱
*   Iconic cartoon graphics 🎨
*   Local Top 10 leaderboard with date/time badges 🏆

## 🏡 What This Mod Adds


### Major New Features

*   **Pre-Game Plant Selection:** Players no longer start with a fixed set of plants. A new **Plant Selection Screen** appears before the game starts, where players must choose a limited deck of plants from a larger library to use in the upcoming match. This adds a significant layer of strategy.
*   **Lawnmowers:** The iconic last line of defense has been added. Each lane is protected by a lawnmower (`🚜`) that will activate upon the first zombie reaching the house, clearing the entire lane once.
*   **Shovel Functionality:** Players can now remove misplaced or unwanted plants using a Shovel (`⛏️`). This is selectable from the plant bar in-game.
*   **Victory Condition:** There is a final wave (Wave 20), and defeating all zombies in that wave now triggers a **Victory sequence**, complete with a collectible trophy (`🏆`) and a victory screen.
*   **Debug/Sandbox Mode:** A hidden zombie spawner has been added, which can be toggled with the 'Z' key. This allows players to manually spawn any type of zombie on any tile for testing or fun.
*   **Custom Dialog System:** Replaces browser alerts/confirms with themed modals for a smoother UX.

---

### Changes to Existing Elements & Mechanics

1.  **Plant Rebalancing and Reworks**
    *   **Chomper (🌿):**
        *   **No Longer Shoots:** The Chomper's ranged attack has been removed.
        *   **New "Chewing" Mechanic:** After eating a zombie, the Chomper is vulnerable and must "chew" for 42 seconds before it can eat again. Its animation now changes to show when it's chewing.
        *   **Anti-Boss Attack:** It cannot eat Gargantuars, but it will bite them for heavy damage at a regular interval.
    *   **Sunflower (🌻):**
        *   **Sun Production Buff:** Sun production has been increased from 40 back to the original **50 sun**.

2.  **Zombie Rebalancing & Toughening**
    *   The health and speed of all original zombies have been significantly increased to make the game more challenging.
    *   **Conehead Zombie (🧟‍♂️):** Health increased from 20 to 28. Speed increased.
    *   **Buckethead Zombie (🧟‍♀️):** Health increased from 40 to 65. Speed increased.
    *   **Pole Vaulting Zombie (💀) (formerly "Fast"):** Health massively increased from 6 to 17. Speed increased.
    *   **Football Zombie (👹) (formerly "Strong"):** Health increased from 60 to 80. Speed increased.

3.  **Core Gameplay Mechanic Changes**
    *   **Plant Cooldowns:** Every plant now has a cooldown period after being planted. You cannot select that plant again until the timer is up, preventing players from spamming powerful units and requiring more forward planning.
    *   **Wave Progression Rework:** The wave system has been fundamentally changed. The primary way to advance is by **defeating all zombies** from the current wave. Once the lawn is clear, the next wave will begin shortly after. This rewards fast and efficient play. A 30-second timer also exists as a backup to ensure the game progresses.
    *   **Advanced Game Engine:** The underlying code for game events, timers, and animations has been completely rewritten into a more robust system. This ensures that all timed events (cooldowns, zombie spawns, sun production) are correctly paused and scaled with the game speed, fixing major bugs in the original.
    *   **Sun Collection Bugfix:** Fixed a bug where you could collect sun multiple times from a single production cycle of a Sunflower.

4.  **UI and UX Enhancements**
    *   **Wave Counter Position:** The wave counter has been moved from the top-right corner to the **bottom-right** for better visibility and to declutter the top UI.
    *   **Sun Collection Animation:** When sun is clicked, it no longer vanishes instantly. It now visually **flies across the screen** and into the sun counter, providing better feedback.

---

### New Plants Added

The arsenal of plants has more than doubled, adding significant strategic variety.

*   **Blover (🍀):** Costs 125 sun. An instant-use plant that creates a strong gust of wind, blowing away all flying Balloon Zombies from the screen instantly.
*   **Cabbage-pult (🥬):** Costs 100 sun. Lobs cabbages at zombies, dealing twice the damage of a standard pea.
*   **Cherry Bomb (💣):** Costs 150 sun. An instant-use plant that explodes, dealing massive damage (90) to all zombies in a 3x3 area. It is consumed on use.
*   **Coffee Bean (☕):** Costs 75 sun. An instant-use plant placed on top of sleeping mushrooms to wake them up for use during the day.
*   **Doom-shroom (🍄):** Costs 125 sun. A highly destructive instant-use plant that explodes in a massive 7x5 area, dealing huge damage (90) to all zombies caught in the blast. It leaves a temporary, unplantable crater at its location.
*   **Garlic (🧄):** Costs 50 sun. A defensive plant that doesn't attack but diverts any zombie that bites it into an adjacent lane.
*   **Gatling Pea (🔫):** Costs 250 sun. An upgrade plant that must be planted on an existing Repeater. It fires a burst of four peas at a time.
*   **Grave Buster (🦇):** Costs 75 sun. A special single-use plant that can only be planted on graves. It consumes the grave over 5 seconds and rewards the player with sun.
*   **Ice-shroom (🧊):** Costs 75 sun. An instant-use plant that freezes every zombie on the entire screen, stopping them in their tracks for 4 seconds and dealing minor damage.
*   **Imitater (🎭):** Cost varies. A strategic plant that transforms into a copy of the previously selected plant card, allowing you to bring two of the same plant into a level with separate cooldowns.
*   **Jalapeno (🌶️):** Costs 125 sun. An instant-use plant that creates a wall of fire, dealing massive damage (90) to and destroying all zombies in an entire lane. It also melts any ice trails left by Zombonis.
*   **Kernel-pult (🌽):** Costs 100 sun. Has a 25% chance to launch butter instead of a kernel. Butter deals more damage and stuns zombies for 5 seconds, temporarily stopping them.
*   **Marigold (🌼):** Costs 50 sun. An economic plant that produces coins instead of sun (described in-game as "useless" for gameplay).
*   **Melon-pult (🍉):** Costs 300 sun. Lobs melons that deal solid damage and splash to nearby zombies on impact.
*   **Potato Mine (🥔):** Costs 25 sun. A cheap, single-use plant that is initially vulnerable. After a 14-second arming time, it will explode on contact, dealing immense damage (90) to a single zombie.
*   **Spikerock (📍):** Costs 125 sun. An upgrade for Spikeweed. It deals more damage and can survive multiple hits from crushing zombies like the Zomboni.
*   **Spikeweed (📌):** Costs 100 sun. A ground-level plant that damages any zombie that walks over it. It cannot be eaten and can be upgraded to Spikerock.
*   **Tall-nut (🌰):** Costs 125 sun. A heavy-duty defensive plant with significantly more health (48) than a Wall-nut, making it an excellent blocker.
*   **Torchwood (🪔):** Costs 175 sun. A supportive plant that turns regular peas passing through it into fire peas, doubling their damage. It also extinguishes freezing projectiles, turning them into normal peas.
*   **Twin Sunflower (🌻🌻):** Costs 150 sun. An upgrade plant that must be planted on an existing Sunflower. It produces 100 sun at a time, doubling the normal rate.
*   **Winter Melon (🥶):** Costs 200 sun. An upgrade for the Melon-pult. Its projectiles deal heavy damage and slow all zombies in the splash zone.
---

### New Zombies Added

The horde has grown much more dangerous and unpredictable.

*   **Football Zombie (👹):** An extremely fast and durable zombie with 80 health. It acts as a battering ram, capable of absorbing a large amount of damage while quickly closing the distance to your house.
*   **Jack-in-the-Box Zombie (🤡):** It moves quickly and has a chance to explode, destroying plants in a 3x3 area around it.
*   **Dancing Zombie (🕺):** A tricky zombie with 17 health. It moves forward with a unique dancing animation and periodically summons four Backup Dancers in the tiles surrounding it, quickly overwhelming a lane.
*   **Backup Dancer (💃):** A standard zombie with 10 health that is only spawned by the Dancing Zombie. They appear in groups and can be very dangerous if the main dancer isn't dealt with quickly.
*   **Zomboni (🚚):** A vehicle-based zombie with 65 health. It moves at a steady pace, instantly crushing any plant it drives over. It also leaves a trail of ice behind it, preventing you from planting on those tiles for a long time.
*   **Balloon Zombie (🎈):** A special zombie with 11 health that floats over all of your plants, making it immune to most attacks. It can only be defeated by the Cactus, Blover, or area-of-effect explosions.
*   **Gargantuar (🗿):** A massive zombie with 150 health that deals devastating damage (99), allowing it to smash plants in a single hit. It is so large that it cannot be eaten by the Chomper.
*   **Giga-Gargantuar (👺):** An even stronger, red-eyed version of the Gargantuar with an immense 300 health, capable of instantly destroying most plants.

---

### New Gameplay Mechanics

*   **Plant Upgrades:** Certain plants (Gatling Pea, Twin Sunflower) can only be planted on top of their base versions.
*   **Instant-Use Plants:** New plants like Cherry Bomb have an immediate, one-time effect.
*   **Special Terrain:** **Graves (`⚰️`), Craters,** and **Ice Trails** now appear on the lawn, blocking planting and affecting strategy.
*   **Flying Zombies:** Balloon Zombies fly over most plants and must be countered specifically.
*   **Zombie Special Abilities:** Zombies can now **crush plants, summon other zombies**.

---

## 💻 Technologies Used

*   **HTML5** for structure
*   **CSS3** for layout & design
*   **JavaScript (ES6)** for game logic

## 📄 License

This project is released under the MIT License. Feel free to use, modify, and distribute.

## 🙏 Acknowledgments

Inspired by the beloved tower defense game *Plants vs. Zombies* by PopCap Games and the [original HTML game](https://github.com/plantsvszombiesjs/plantsvszombiesjs.github.io).

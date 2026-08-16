# 🔵 Dodge Game

A simple **2D Dodge Game built with Python and Pygame**.

The player controls a blue square and must avoid red enemy squares that move around the screen. The enemies bounce off the walls, and their speed increases every few seconds, making the game progressively more difficult.

The objective is simple: **survive for as long as possible and achieve the highest score.**

---

## 🎮 Game Features

* 🔵 Player-controlled character
* 🔴 Multiple moving enemies
* 🧱 Enemies bounce off the screen boundaries
* 💥 Collision detection
* ⏱️ Time-based scoring system
* 📈 Enemy speed increases every 5 seconds
* 🎯 Increasing difficulty
* 🖥️ 800 × 600 game window
* ⚡ Runs at 60 FPS
* 🚪 Game Over system

---

## 🛠️ Technologies Used

* **Python 3**
* **Pygame**
* `random` — for random enemy positions and directions
* `sys` — for safely exiting the game

---

## 📁 Project Structure

```text
Dodge-Game/
│
├── main.py
└── README.md
```

---

## ⚙️ Requirements

Make sure Python 3 is installed on your system.

Install Pygame using:

```bash
pip install pygame
```

If your system uses `pip3`:

```bash
pip3 install pygame
```

---

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone https://github.com/your-username/Dodge-Game.git
```

### 2. Open the project directory

```bash
cd Dodge-Game
```

### 3. Install Pygame

```bash
pip install pygame
```

### 4. Run the game

```bash
python main.py
```

---

## 🎮 Controls

| Key            | Action     |
| -------------- | ---------- |
| ⬆️ Up Arrow    | Move Up    |
| ⬇️ Down Arrow  | Move Down  |
| ⬅️ Left Arrow  | Move Left  |
| ➡️ Right Arrow | Move Right |
| ❌ Close Window | Exit Game  |

---

## 🕹️ How to Play

1. Start the game.
2. Control the **blue square** using the arrow keys.
3. Avoid the **red enemy squares**.
4. Enemies move continuously and bounce off the screen edges.
5. Your score represents the number of seconds you survive.
6. Every **5 seconds**, the enemy speed increases.
7. If the player collides with an enemy, **GAME OVER** is displayed.
8. The game closes after the Game Over screen.

---

## 📊 Scoring System

The score is based on the amount of time the player survives.

```text
Score = Time Survived (seconds)
```

For example:

```text
Score: 10
```

means the player survived for approximately **10 seconds**.

---

## 📈 Difficulty System

The game becomes progressively harder.

Initially:

```python
enemy_speed = 6
```

Every 5 seconds, the speed increases by 1:

```python
enemy_speed += 1
```

Therefore, the longer you survive, the faster the enemies become.

Example:

| Survival Time | Enemy Speed |
| ------------: | ----------: |
|       0–5 sec |           6 |
|      5–10 sec |           7 |
|     10–15 sec |           8 |
|     15–20 sec |           9 |
|     20–25 sec |          10 |

---

## 💥 Collision Detection

The game uses Pygame's `Rect.colliderect()` function to detect collisions between the player and enemies.

```python
if player_rect.colliderect(enemy["rect"]):
```

When a collision occurs:

```text
GAME OVER
```

is displayed and the game exits after a short delay.

---

## 🎨 Game Objects

### 🔵 Player

The player is represented by a blue square.

```python
player_size = 50
player_speed = 6
```

### 🔴 Enemies

Enemies are represented by red squares.

There are currently **2 enemies**:

```python
enemy_count = 2
```

Their starting positions and movement directions are randomly generated.

---

## 🧠 Concepts Demonstrated

This project demonstrates several important Python and game-development concepts:

* Python game loops
* Pygame initialization
* Keyboard input handling
* Random number generation
* Object movement
* Screen boundary detection
* Wall bouncing
* Collision detection
* Time tracking
* Dynamic difficulty
* Score calculation
* Event handling
* Frame-rate control
* Program termination

---

## 🔮 Future Improvements

Possible improvements for future versions include:

* 🖼️ Add player and enemy images
* 🔊 Add sound effects
* 🎵 Add background music
* 🏆 Add a high-score system
* 🔄 Add a restart button
* ❤️ Add multiple lives
* 👾 Add more enemy types
* 🎨 Add a better background
* 📋 Add a main menu
* ⏸️ Add a pause system
* 📈 Add difficulty levels
* 💫 Add animations and particle effects
* 🥇 Save the highest score to a file



## 👨‍💻 Author

**Naman Karna**

A simple Python/Pygame project created for learning and practicing game development.

---

## 📄 License

This project is intended for **educational and personal use**.

Feel free to modify the code, experiment with new features, and use it as a starting point for your own Pygame projects.

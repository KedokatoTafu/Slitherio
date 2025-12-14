# 🐍 Slither.io
A replica of the popular multiplayer arcade game Slither.io, built entirely with Python and Pygame.

I developed this project to help me understand game development fundamentals, specifically focusing on handling real-time rendering, vector mathematics for movement logic, and object-oriented design for managing game entities (AI agents and the player).

## 🛠 Technologies
* **Python**

* **Pygame**

## ✨ Features
🎮 **Gameplay Mechanics**
* **Smooth Movement:** Snake movement is calculated using vectors, allowing for 360-degree turning radius controlled by the mouse cursor.

* **Dynamic Camera:** Implemented a Camera class that centers the viewport on the player while allowing them to explore a game world much larger than the window size.

* **Growth System:** Snakes grow in length (Segment.py) dynamically as they consume orbs scattered around the map.

* **Collision Detection:** Precise hitbox detection determines when a snake runs into another snake's body, triggering a "Game Over" or eliminating the AI.

🤖 **Artificial Intelligence** (Not really)
* **Autonomous Agents:** The game features CPU-controlled snakes that wander the map, hunt for food, and interact with the player.

* **Behavior Logic:** AI calculates directions based on random wandering or target tracking algorithms.

🎨 **Rendering**
* **Custom Textures:** Rendering distinct skins for the player and enemies using loaded assets (textures/).

* **UI Elements:** On-screen score tracking and leaderboard display using FontRenderer.py.

## 🚀 The Process
* **Core Engine Setup:** I started by initializing the Pygame window and creating the main game loop (main.py & MainGame.py) to handle frame updates (FPS).

* **Entity Modeling (OOP):** I created a base Object class, then extended it for Snake, which is further specialized into Player and AI. This inheritance structure reduced code duplication significantly.

* **Movement Logic:** Implementing the snake's "slithering" effect was the hardest part. I used vector math to make the body segments follow the head's path with a slight delay, creating a natural trailing animation.

* **Camera System:** To simulate a large map, I wrote a Camera class that calculates offsets. Instead of moving the player, the world moves around the player.

* **AI Implementation:** Finally, I added AI bots to make the game feel alive, programming them to move within the map boundaries.

## 🧠 What I Learned
* **Vector Mathematics:** I gained a practical understanding of vectors (normalizing, scaling) to calculate direction and velocity.

* **Game Loop Architecture:** I learned the update-render cycle: Handle Input -> Update Logic -> Draw Frame.

* **State Management:** Learned how to manage dynamic lists of objects (adding/removing food and snakes) without causing memory leaks or performance drops.

* **Pygame Proficiency:** Improved my knowledge of blitting images, surface manipulation, and event listeners.

🔮 How can it be improved?
* **Network Multiplayer:** Implement socket programming to allow real players to connect via LAN or Internet.

* **Optimization:** Implement "Quadtrees" for collision detection to improve performance when there are hundreds of entities on screen.

* **Power-ups:** Add speed boost mechanics (consuming mass to move faster).

## 🏃 Running the Project
To run the project in your local environment, follow these steps:
  1. Ensure you have Python installed.
  2. Install Pygame:
       ```
       pip install pygame
       ```
  4. Run the game:
       ```
       cd Slitherio
       python main.py
       ```

## 🖼 Views
<img width="975" height="564" alt="image" src="https://github.com/user-attachments/assets/018e4b92-051b-4260-8cc7-559e93409d04" />

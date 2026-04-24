# Pac-Man AI Project

This project is a classic Pac-Man game where the Artificial Intelligence (AI) plays the game automatically to collect points and run away from ghosts.

---

## Authors
* **Abdelrahman Askar**
* **Ali Emad**

---

## AI Algorithms Used
We used a combination of **Depth-Limited Search (DLS)** and a **Heuristic Evaluation (Greedy approach)** for the AI in this project.

### Why did we use DLS and Heuristic?
Standard algorithms like normal BFS, DFS, or A* would take too much memory and time to check the entire map for every single frame, which causes the browser game to freeze. We used DLS and Heuristics because:
1. **Performance (DLS):** Instead of searching the whole map to find the ultimate end goal, Pac-Man only looks ahead for a specific limited number of steps (depth limit). This keeps the game running very fast and smoothly in real-time.
2. **Smart Decisions (Heuristic & Greedy):** After looking ahead, the AI gives a "Score" (Heuristic value) to each possible path. A path gets a high score if it has a lot of dots, fruits, energizers, or is far away from dangerous ghosts. Pac-Man then greedily chooses the path with the highest score.
3. **Ghost Avoidance:** The AI can predict ghost movements. If a path leads to a ghost, the score drops drastically, forcing Pac-Man to quickly pick a safer route.

---

### Where is the Algorithm in the Code?
The algorithm logic is implemented inside the player code. The AI calculates future paths up to the specific depth limit, evaluates them using the heuristic scoring system, and chooses the best and safest path.

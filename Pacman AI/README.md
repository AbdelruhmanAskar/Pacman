# Pac-Man AI Project

This project is a classic Pac-Man game where the Artificial Intelligence (AI) plays the game automatically to collect points and run away from ghosts.

---

## Authors
* **Abdelrahman Askar**
* **Ali Emad**

---

## AI Algorithm Used
We used the **A* (A-Star) Search Algorithm** for the AI in this project.

### Why did we use A* Search?
A* is the smartest and most efficient algorithm for pathfinding in games like Pac-Man. We used it because:
1. **Shortest Path:** It always finds the shortest and fastest way to eat dots and energizers.
2. **Smart Decisions:** It uses a "Heuristic" (a smart guess) to know which direction is closer to the target without checking every single path. This makes it very fast.
3. **Safety:** It can easily calculate the cost of moving. If there is a ghost in the way, A* will see that path as "too expensive" or dangerous and will quickly find a safer alternative route to survive.

---

### Where is the Algorithm in the Code?
The algorithm logic is implemented inside the player and AI behavior files. It calculates all possible future moves, gives them a score based on distance and safety (Heuristic), and then chooses the best move to keep Pac-Man alive and winning.

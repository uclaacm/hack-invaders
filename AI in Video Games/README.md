AI in Video Games
> Presentation by Max Zhang
https://docs.google.com/presentation/d/1obqCDoOAow1sgE_ZoCfYlibCCxuE7ojKzfHU-a9UyyI/edit?slide=id.g3e7f0f034f0_0_0#slide=id.g3e7f0f034f0_0_0


**Overview**

AI in gaming philosophy: creating NPCs that simulate human players. 
There are two broad categories — **Classic AI** and **Modern AI**. 

---

## Classic AI — Concrete Rules Dependent

Best used in games with well-defined rules (e.g. Tetris, Sudoku, Pac-Man).

**Pros:** Easy to implement, predictable, no training data required.  
**Cons:** Can feel repetitive, can't handle unexpected scenarios, requires manual updates for new situations.

### Core Techniques
 
**Finite State Machines (FSM)** - Characters switch between a limited set of states that define their behavior. Example: Pac-Man ghosts have Chase, Scatter, and Frightened states.
 
**Pathfinding Algorithms** - Find the fastest route from point A to B. Key algorithms include Dijkstra and A* (A-star). Example: Ghost chasing Pac-Man through the maze.
 
**Decision Trees & If/Else Logic** - Choose the best action given the current situation and available resources. Example: Tic-Tac-Toe AI.
 
**Heuristics & Scoring Systems** - Evaluate which action yields the best value when there are too many options for a full search. Uses Min-Max algorithms. Example: Chess AI.
 
___________________________________________________

## Modern AI — Adaptability

Best used in games centered around dynamic user inputs (e.g. Snake, Mario Kart).

**Pros:** More variation, greater adaptability, handles unexpected inputs.  
**Cons:** Hard to control, requires large amounts of data, more complex to implement.

### Core Techniques
 
**Reinforcement Learning (RL)**- Trains a model on past data by rewarding good behaviors and penalizing bad ones. Example: Driving simulators.
 
**Generative AI** - Dynamically generates images, music, or text based on the current game state using tools like DALL-E, Stable Diffusion, or LLMs. Example: Adaptive storytelling.
 
**Neural Network Behavior (Learned NPCs)** - Like RL, but NPCs train in real time on live player input rather than pre-collected data. Example: Donkey Kong anticipating a player jump.

## Resources

**Pathfinding**
- A* Algorithm — fastest, but information-heavy
- Dijkstra's Algorithm — simpler alternative

**Decision Making**
- Minimax Algorithm
- Finite State Machines

**Image & Art Generation**
- DALL-E 3 (OpenAI)
- Stable Diffusion via Replicate
- Ideogram / Playground AI

**Text & Logic**
- Anthropic Claude API

**In-Browser Machine Learning**
- ML5.js
- TensorFlow.js

**Reinforcement Learning**
- Phaser + RL
- Python + Pygame + Gymnasium

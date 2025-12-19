# CS 370 – Pirate Intelligent Agent (Deep Q-Learning)

## Project Overview
This project implements a pirate non-player character (NPC) for a treasure hunt game using **deep reinforcement learning**. The goal of the intelligent agent is to navigate a maze-based environment and consistently reach the treasure before a human player. The project demonstrates the application of **deep Q-learning**, **neural networks**, and **experience replay** to solve a pathfinding problem.

The primary artifact for this project is a Jupyter Notebook that trains and evaluates the pirate agent using a Deep Q-Network (DQN).

---

## Work Completed in This Project

### Provided Code
The starter code included:
- `TreasureMaze.py`, which defines the game environment, maze layout, rewards, valid actions, and terminal states.
- `GameExperience.py`, which manages experience replay memory and prepares training data.
- A partially completed Jupyter Notebook with helper functions, visualization tools, and a skeleton for the training loop.

These files defined the environment and constraints but did not include a complete learning algorithm.

### Code I Implemented
I implemented the **core deep Q-learning training algorithm** inside the `qtrain()` function. My work included:
- Designing the training loop that resets the environment at random starting positions
- Implementing **epsilon-greedy exploration vs. exploitation**
- Storing state transitions in an experience replay buffer
- Training a neural network to approximate Q-values
- Periodically updating a target network for training stability
- Tracking performance metrics such as loss, win rate, and episode count
- Validating the trained agent using a completion check across all valid starting positions

The final result is an agent that reliably achieves a **100% win rate**, demonstrating successful learning and generalization across the maze.

---

## Connection to Computer Science

### What Do Computer Scientists Do and Why Does It Matter?
Computer scientists design algorithms and systems that solve complex problems efficiently and reliably. In this project, I applied theoretical concepts from artificial intelligence and machine learning to build a system that can learn from experience rather than relying on hardcoded rules. This approach matters because many real-world problems—such as robotics, game AI, and autonomous systems—require adaptability in dynamic environments.

### How I Approach a Problem as a Computer Scientist
I approach problems by first understanding the constraints and goals of the system, then selecting an appropriate algorithmic approach. For this project, I identified reinforcement learning as the correct paradigm for a pathfinding problem with delayed rewards. I broke the problem into smaller components—state representation, action selection, reward structure, and learning—and iteratively refined the solution through testing and evaluation.

### Ethical Responsibilities to Users and Organizations
When designing intelligent systems, I have an ethical responsibility to ensure transparency, reliability, and responsible use. In game AI, this includes avoiding unfair advantages, ensuring predictable behavior, and preventing systems from exploiting unintended mechanics. More broadly, the same reinforcement learning techniques used here can be applied in sensitive domains, making it essential to consider bias, misuse, and unintended consequences when deploying AI systems.

---

## Technologies and Concepts Used
- Python
- TensorFlow / Keras
- Deep Q-Learning (DQN)
- Neural Networks
- Experience Replay
- Reinforcement Learning
- Epsilon-Greedy Exploration
- AI Pathfinding

---

## Repository Contents
- `TreasureHuntGame_starterCode.ipynb` – Jupyter Notebook containing the trained pirate intelligent agent
- `TreasureHuntGame_starterCode.html` – Exported HTML version of the notebook
- `TreasureMaze.py` – Game environment (provided)
- `GameExperience.py` – Experience replay logic (provided)
- `requirements.txt` – Project dependencies (provided)
- `README.md` – Project description and reflection

---

## Author
**Carlos Trujillo**  
Computer Science Student  
Focus areas: Artificial Intelligence, Game Development, Software Engineering

# 🐦 Flappy Bird AI - Deep Q-Learning

## 🎮 Overview
This project is an implementation of a Deep Q-Network (DQN) to teach an agent how to play the famous game Flappy Bird using PyTorch and PyGame. The agent interacts with the game environment and learns optimal actions through Q-learning to achieve the highest possible score.

## 🚀 Features
- **Deep Q-Learning**: Utilizes both DQN and Double DQN (DDQN) for stable training.
- **Experience Replay**: Memory buffer stores agent experiences for sampling and training to break the correlation between sequential data.
- **Target Network**: Separate target network for calculating stable Q-value updates.
- **Epsilon-Greedy Policy**: Balances exploration and exploitation by decaying the epsilon value over time.

## 🧠 Algorithms
The agent is trained using the Q-learning algorithm, where the Q-value of each action is updated based on the reward received from the environment.

- **State Representation**: The state is represented as a vector of game variables such as bird’s position, velocity, and distance from pipes.
- **Action Space**: The agent chooses between two possible actions: flap or no flap.
- **Reward Function**: The agent receives a reward for surviving longer and a penalty when it crashes.

## 📊 Performance
The agent’s performance improves over time. Below are some sample results from the training process:

- **Score vs Episode**
- **Episode Duration vs Episode**

As you can see from the plots, the agent gradually learns to survive longer and improve its score through training.

## 🛠️ Installation & Setup
1. Clone the repository
    ```bash
    https://github.com/Samridhi1412/FlappyBird.git
    cd Flappy_Bird_AI
    ```
2. Install dependencies
    ```bash
    pip install -r requirements.txt
    ```
3. Run the training
    To train the agent, simply run:
    ```bash
    python train.py
    ```
4. Watch the agent play!
   Once training is complete, you can watch the agent play the game by running:
    ```bash
    python play.py
    ```

## 📁 Project Structure
- `main.py`: The entry point of the project that initializes the environment, sets up the game, and trains the agent.
- `model.py`: Defines the architecture of the deep Q-network used by the agent.
- `memory_recall.py`: Implements experience replay using a deque to store agent’s experiences.
- `agent.py`: Contains the core agent logic, including action selection, experience caching, and model optimization.
- `train.py`: Script for training the agent with the game environment.
- `play.py`: Script to watch the trained agent play the game.

## 🏆 Results
After several episodes of training, the agent learns to avoid pipes and score higher. Here's an example of the agent achieving a high score:

## 📊 Performance
The agent’s performance improves over time. Below are some sample results from the training process:

### Score vs Episode
![Score vs Episode](path/to/score_vs_episode.pngC:\Users\KIIT\OneDrive\sco vs episode.png)

### Episode Duration vs Episode
![Episode Duration vs Episode](path/to/score_vs_episode.pngC:\Users\KIIT\OneDrive\dur vs epi.pngs)

As you can see from the plots, the agent gradually learns to survive longer and improve its score through training.

## 📜 License
This project is licensed under the MIT License.

# CS370_Current-Emerging_Trends
CS-370 Current Emerging Trebds

The project for this class involves implementing deep Q-learning for a treasure hunt game where a pirate agent aims to find the treasure before the pirate does. Here's an overview of the work done on this project:

1. **Maze Definition:** An 8x8 maze is defined as a numpy array, representing the game environment. It contains cells with values 0 (free cells), 1 (obstacles), and 2 (treasure).

3. **Helper Functions:** There are functions for visualizing the maze and performing actions in the environment. These functions are used for testing and visualization.

4. **Q-Learning Parameters:** Parameters like exploration factor (epsilon), action dictionary, and the number of possible actions are defined. Actions are represented as integers (LEFT, UP, RIGHT, DOWN).

5. **Game Simulation:** Functions are provided for simulating a game based on a trained model and checking if the pirate can win any game at all.

6. **Neural Network Model:** A neural network model is constructed using Keras. It has several dense layers with activation functions and is compiled with the mean squared error loss function for Q-learning.

7. **Deep Q-Learning Implementation:** The main part of the project involves implementing deep Q-learning using the provided pseudocode. The algorithm includes the following steps:
   - Randomly selecting a free cell as the starting position for the pirate agent.
   - Resetting the maze with the agent at the selected cell.
   - Using an epsilon-greedy strategy to decide whether to explore or exploit.
   - Collecting episodes (previous state, action, reward, new state, game status).
   - Storing episodes in an experience replay object.
   - Training the neural network model with experience replay data.
   - Calculating the win rate and adjusting epsilon.
   - Checking for a high win rate and completion of the maze.

8. **Testing the Model:** After training, the code tests the model by creating an instance of TreasureMaze, building the model, and running the Q-learning training process. It then checks if the model passes the completion check and simulates a game to see if the agent can find the treasure.

9. **Save and Submit:** Finally, the code suggests saving the notebook with a specific filename and submitting it for evaluation.

As a computer scientist, the work on this project demonstrates several key concepts:

- **Problem Solving:** Computer scientists analyze problems, break them down into manageable components, and devise algorithms to solve them. In this project, the problem is to teach an agent to navigate a maze and find a treasure, which requires designing and implementing a deep Q-learning algorithm.

- **Machine Learning:** Computer scientists use machine learning techniques to build intelligent agents that can learn from data and make decisions. Deep Q-learning is a machine learning approach used in this project to train the pirate agent.

- **Algorithm Design:** Designing efficient and effective algorithms is a fundamental skill for computer scientists. The Q-learning algorithm is a crucial part of this project's implementation.

- **Data Handling:** Computer scientists work with data, and in this project, data is collected in the form of episodes and used for training and evaluation.

Regarding ethical responsibilities, computer scientists must consider the following:

- **Transparency and Accountability:** When designing AI systems, it's essential to ensure transparency in how the system makes decisions and to be accountable for any biases or errors that may arise.

- **Data Privacy:** If the project involves user data, it's crucial to protect user privacy and handle data ethically, following privacy laws and best practices.

- **Fairness:** Ensure that the AI system treats all users and stakeholders fairly and does not discriminate based on sensitive attributes like race, gender, or religion.

- **Safety:** Consider the safety of the AI system and its impact on users. Ensure that it does not pose physical or psychological harm.

- **Impact on Society:** Consider the broader societal implications of the AI system and how it may affect individuals and communities.

In summary, computer scientists work on various aspects of problem-solving, algorithm design, machine learning, and ethical considerations in the development of AI systems, as demonstrated in this project.

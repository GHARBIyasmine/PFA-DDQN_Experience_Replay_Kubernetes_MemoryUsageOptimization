# PFA-DDQN_Experience_Replay
This repository provides code and resources for a Double Deep Q-Network (DDQN) with Experience Replay, a deep reinforcement learning (DRL) solution for load optimization in edge Kubernetes clusters. It aims to enhance Kubernetes efficiency and performance by dynamically managing and redistributing workloads based on real-time memory usage across nodes.

## Key Features
- **Double Deep Q-Network (DDQN)**: Utilizes a DDQN architecture to enhance the stability and performance of the learning process by addressing the overestimation bias often found in standard DQNs.
- **Experience Replay** : Implements an experience replay mechanism to store and reuse past experiences, which helps in breaking the correlation between consecutive experiences and improves learning efficiency.
- **Kubernetes Environment Simulation**: Contains a training environment code that simulates a Kubernetes cluster, providing a realistic setting for training the DRL agent.
- **Load Optimization**: Focuses on optimizing memory usage across nodes in the cluster, ensuring balanced and efficient workload distribution to prevent memory bottlenecks and improve overall cluster performance.

## Notebook Architecture
1. **Pod model desciption** : 
Details the modeling of jobs and pods within the Kubernetes environment.
2. **Define Imports** :
Contains the necessary imports and dependencies required for the project.
3. **Cluster Simulation** :
Simulates the Kubernetes cluster environment, providing a realistic setting for training the DRL agent whci inlcudes :

   3.1 **Pod class**
   
   3.2 **Node class**

   3.3 **Cluster class**

   3.4 **Reward Functions** : Defines the reward functions used to guide the agent's learning process.
             
5. **Agent Class** :
Implements the DDQN agent, encapsulating the core logic of the learning algorithm.
6. **Experience Replay** :
Implements the experience replay mechanism to store and reuse past experiences.
7. **Environment Class** :
Defines the environment class that interacts with the DDQN agent, simulating the Kubernetes cluster's state and transitions.
8. **main class** :
The main class orchestrates the training process, integrating all components and executing the training loop.


## Prerequisites
- Python 3.10.14
- Jupyter Notebook
- TensorFlow 2.10.1
- Numpy 1.26.4
- Kubernetes cluster (simulated or real) for testing and deployment

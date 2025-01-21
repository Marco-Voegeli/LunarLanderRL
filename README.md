# VPG Algorithm with Actor-Critic Architecture

This repository implements a Vanilla Policy Gradient (VPG) reinforcement learning algorithm using a neural network-based Actor-Critic architecture. The implementation is tested on the LunarLander-v3 environment.

## Features

- **Actor-Critic Architecture**: Combines a policy network (actor) and a value function network (critic).
- **Advantage Estimation**: Uses Generalized Advantage Estimation (GAE) for stabilizing policy gradient updates.
- **Multilayer Perceptron (MLP)**: Customizable neural networks for policy and value function.
- **Policy and Value Function Updates**: Separate optimization steps for actor and critic networks.
- **Environment Support**: Tested on LunarLander-v3 environment with Gymnasium API.

## Results

- **Policy Performance**: The trained policy achieves a mean return of approximately 200 on the LunarLander-v3 environment.
- **Videos**: Recorded videos of the trained policy are saved in the `policy_videos` folder.

### Visualization Outputs

- **Policy Rollouts**: Recorded videos of agent performance.

  

https://github.com/user-attachments/assets/9de1a299-9d1e-4fc5-a239-3180bedc4755



## Prerequisites

Install the required dependencies:

```bash
pip install numpy torch gymnasium matplotlib scipy
```

## Usage

1. Train the agent by running the main script:

```bash
python solution.py
```

2. Evaluate the trained policy by observing its performance in the LunarLander-v3 environment. Videos of policy rollouts will be saved in the `policy_videos` directory.

3. Adjust hyperparameters (e.g., learning rates, network sizes) directly in the `Agent` class to experiment with different setups.

## File Structure

- `solution.py`: Main implementation of the VPG algorithm with actor-critic architecture.
- `policy_videos`: Directory containing recorded videos of the trained policy.

## Author

This repository demonstrates reinforcement learning using policy gradient methods with neural networks.

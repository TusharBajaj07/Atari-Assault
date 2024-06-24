# Assault-v5 Reinforcement Learning Agent

This repository contains a reinforcement learning agent interacting with the "Assault-v5" environment from the Arcade Learning Environment (ALE) using OpenAI's Gym.

## Requirements

- Python 3.8+
- OpenAI Gym
- PyTorch
- torchvision

For detailed instructions on setting up your environment, watch this video: [How to Setup Your Environment](https://youtu.be/gMgj4pSHLww?si=xq3wESPpZe6HmgWz)


## Code Overview

### Environment Setup
- Initializes the "Assault-v5" environment with human rendering mode.
- Resets the environment to obtain the initial observation and info.

### Main Loop
- The agent takes random actions sampled from the environment's action space for 1000 steps.
- For each step, the environment returns the new observation, reward, termination flag, truncation flag, and additional info.
- If the episode is terminated or truncated, the environment is reset.

### Model and Data Processing
- The observation is normalized and converted to a tensor.
- A PyTorch DataLoader is prepared (currently commented out in the code).
- Augmentations are applied to the observations using torchvision transforms.
- A neural network model processes the observation tensor.

### Environment Closure
- The environment is closed after the loop completes.


#### Video explanation link [Code Explanation](https://drive.google.com/drive/folders/1fE2viRx0kIoLONUnnNXeGx1PNrwuvpvJ?usp=drive_link)

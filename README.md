# LLM-Guided Reinforcement Learning for Robotic Manipulation

## Description
A minimal proof-of-concept that pairs a large language model (LLM) with reinforcement learning (RL) to control a 6-DOF robotic arm in simulation.  
The LLM proposes either joint commands or end-effector poses; RL then refines these actions via trial-and-error rewards.

## Goal
Pick up and lift a single cube in the ManiSkill2 simulator >80 % of test runs, while keeping the controller fully interpretable (LLM prompts + rewards).

## Steps
1. **Setup**  
   ```bash
   conda env create -f env.yml        # install PyTorch + ManiSkill2 etc.
   conda activate llm-rl

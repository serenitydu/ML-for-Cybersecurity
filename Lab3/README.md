# Lab 3 report

@Author: Chenghao Du\
@Time: 2021/12/16

## Description
1. Download model, weights, and data mentioned in `Lab_README.md`, and put them in the correct folder.
2. Run `BadNet.ipynb` in Jupyter notebook.

## Pruning defense comments
The pruning defense does not work for this model. Here are two possible clues that may cause this problem:\
1. The CA decrases faster than ASR when we punish weights. When CA decreased to 60%, the ASR is still at 98%.
2. If we take a look at the dataset, we will notice that the 'poisoned glasses' takes over almost 1/2 of the image  pixels, so it will highly influence the weights when attackers train the 'BadNet' using bad data.


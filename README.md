# TransferRL-on-Gfootball
Trained GFootball environment on different tasks. Trained on 3_vs_1 first from scratch. Then trained 5_vs_3 on parameters from 3_vs_1 and scratch. While there was no difference in the time taken to achieve more than 95% performance, the transfer learned model learned passing from the previous model while the model trained from scratch opted to dribble. The goal of this training was to figure out if there is a way to make RL models learn concepts rather than overfit on the environment. The next step would be to use this learning paradigm to make RL agent learn relations among entites in environment.
# Implementation:
The agent architecture used was that of IMPALA CNN architecture. There were in total of 19 layers which consisted of convolution, residual blocks and fully connected layers. There were also multiple environments created in parallel but the entire model was synchronous. Also all the environments followed the same policy but at different points in the environment.
# Training results


| ![3_vs_1](https://github.com/aveen-d/TransferRL-on-Gfootball/blob/master/gifs/3_v_1.gif) |  
|--|
| 3_vs_1 from scratch | 

| ![5_vs_3_scratch](https://github.com/aveen-d/TransferRL-on-Gfootball/blob/master/gifs/5_v_3_scratch.gif) | ![5_vs_3_transfer](https://github.com/aveen-d/TransferRL-on-Gfootball/blob/master/gifs/5_v_3_transfer.gif) |
|--|--|
| 5_vs_3 from scratch | 5_vs_3 transfer learned  |

| ![](https://github.com/aveen-d/TransferRL-on-Gfootball/blob/master/Graphs/1.png) | ![](https://github.com/aveen-d/TransferRL-on-Gfootball/blob/master/Graphs/2.jpg) | ![](https://github.com/aveen-d/TransferRL-on-Gfootball/blob/master/Graphs/3.jpg) |
|--|--|--|
|  |  |  |

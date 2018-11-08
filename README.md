Abstract
========

Robot navigation is a fundamental problem in robotics and various approaches have been developed to cope with this problem. Despite the great success of previous approaches, learning-based methods are receiving growing interest in the research community. They have shown greater efficiency in solving navigation tasks and offer considerable promise to build intelligent navigation systems. This paper presents a goal-directed robot navigation system that integrates global planning based on goal-directed end-to-end learning and local planning based on reinforcement learning. The proposed system aims to navigate the robot to desired goal positions while also being adaptive to changes in the environment. The global planner is trained to imitate an expert's navigation between different positions by goal-directed end-to-end learning, where both the goal representations and local observations are incorporated to generate actions. However, it is trained in a supervised fashion and is weak in dealing with changes in the environment. To solve this problem, a local planner based on deep reinforcement learning is designed. The local planner is first implemented in a simulator and then transferred to the real world. It works complementarily to deal with situations that have not been met during training the global planner and is able to generalize over different situations. The experimental results on a robot platform demonstrate the effectiveness of the proposed navigation system.


The proposed navigation system consists of a global planner and a local planner which are based on two learning methods: end-to-end learning and reinforcement learning (D3QN).

Goal-directed end-to-end learning
========

<img src="https://github.com/xiaomaozhou26/Towards-Goal-Directed-Navigation-Through-Combining-Learning-Based-Global-and-Local-Planners/blob/master/vgg_action1.jpg"  width="720" height="450">

Training Data 
========
The training data is collected in our lab.

D3QN
========
<img src="https://github.com/xiaomaozhou26/Towards-Goal-Directed-Navigation-Through-Combining-Learning-Based-Global-and-Local-Planners/blob/master/ddqn1.jpg"  width="920" height="450">

Reference
========
1. Codevilla F, Miiller M, López A, et al. End-to-end driving via conditional imitation learning[C]//2018 IEEE International Conference on Robotics and Automation (ICRA). IEEE, 2018: 1-9.
2. Xie L, Wang S, Markham A, et al. Towards monocular vision based obstacle avoidance through deep reinforcement learning[J]. arXiv preprint arXiv:1706.09829, 2017.

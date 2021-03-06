# Unity Machine Learning Agent

## Introduction

This is repository for **Unity Machine Learning Agent** and **Reinforcement Learning(RL)**.

Unity release awesome tool for making reinforcement learning environment! [Unity Machine Learning](https://unity3d.com/machine-learning)

I usually make 2D RL environment with [pygame](http://www.pygame.org/news). [pygame environment repository](https://github.com/Kyushik/DRL)

Thanks to Unity, I am trying to make some 3D RL Environments.

I wrote summary of RL algorithms in [pygame environment repository](https://github.com/Kyushik/DRL)



Some of the environment made by purchased models. In this case, it is hard to provide raw unity codes. However, there are some simple environments which are made by simple or free model. I will provide raw unity codes for those environments if I solve the capacity problem.



### Environment

**Software**
* Windows7 (64bit), Ubuntu16.04
* Python 3.5.2
* Anaconda 4.2.0
* Tensorflow-gpu 1.3.0
* Unity version 2017.2.0f3 Personal
* opencv3 3.1.0

**Hardware**
* CPU: Intel(R) Core(TM) i7-4790K CPU @ 4.00GHZ

* GPU: GeForce GTX 1080Ti

* Memory: 8GB

  ​


### UnityEnv

I added some environments and assets for making ML-agents

- ML-agents: It is basic ML-agent v0.3 environment from [official ML-agents github](https://github.com/Unity-Technologies/ml-agents)
- Assets: assets for making games 



## Unity ML Environments

### Deep Q Learning Based High Level Driving Policy Determination

<img src="./Images/Simulator_sample.PNG" width="500" alt="Vehicle_Simulator_StaticObs" />



This project was one of the project of [Machine Learning Camp Jeju 2017](http://mlcampjeju.kakao.com/).

After the camp, simulator was changed to [Unity ML-Agents](https://unity3d.com/machine-learning). Also, I wrote a paper about this project and it accepted to [Intelligent Vehicle Symposium 2018](http://www.2018iv.org/)

The Repository link of this project as follows. 

[Repository Link!!!](https://github.com/MLJejuCamp2017/DRL_based_SelfDrivingCarControl)

---

### Vehicle Environment(Dynamic Obstacles)

<img src="./Images/Vehicle_environment_dynamic.PNG" width="500" alt="Vehicle_Simulator_DynamicObs" />

 

 The agent of this environment is vehicle. Obstacles are other 8 different kind of vehicles. If vehicle hits other vehicle, it gets minus reward and game restarts. If vehicle hits start, it gets plus reward and game goes on.  The specific description of the environment is as follows.



Above demo, referenced papers to implement algorithm are as follows.

- [Dueling Network Architectures for Deep Reinforcement Learning](https://arxiv.org/abs/1511.06581)




Download links of this environments are as follows.

- Vehicle Environment Dynamic Obs Windows [Link](https://www.dropbox.com/s/cnhe9ip7e7hviff/ML_Agent_VehicleEnvironment_dynamic_windows.zip?dl=0)
- Vehicle Environment Dynamic Obs Mac [Link](https://www.dropbox.com/s/7bk6ffp6jmg4je3/ML_Agent_VehicleEnvironment_dynamic_mac.zip?dl=0)
- Vehicle Environment Dynamic Obs Linux [Link](https://www.dropbox.com/s/i4qghzby3jmz6nz/ML_Agent_VehicleEnvironment_dynamic_linux.zip?dl=0)

---

### Vehicle Environment(Static Obstacles)

<img src="./Images/Vehicle_Simulator_static_sample_img.jpg" width="500" alt="Vehicle_Simulator_StaticObs" />

 

Yeah~~ This environment won [ML-Agents Challenge](https://blogs.unity3d.com/kr/2018/02/28/introducing-the-winners-of-the-first-ml-agents-challenge/?_ga=2.161712891.672728060.1524014504-1436221211.1493602207)!!! :crown:



 The agent of this environment is vehicle. Obstacles are static tire barriers. If vehicle hits obstacle, it gets minus reward and game restarts. If vehicle hits start, it gets plus reward and game goes on.  The specific description of the environment is as follows.

- [Specific description of the environment](https://github.com/Kyushik/Unity_ML_Agent/blob/master/VehicleEnv_static.md)




Sample video of this game is as follows.

Game demo [youtube video](https://youtu.be/-LbuCPwiSVY) 

Above demo, referenced papers to implement algorithm are as follows.

- [Noisy Networks for Exploration](https://arxiv.org/abs/1706.10295)
- [Deep Reinforcement Learning with Double Q-learning](https://arxiv.org/abs/1509.06461)





Download links of this environments are as follows.

- Car Game Static Obs Windows [Link](https://www.dropbox.com/s/eaxq55kjm80nnsp/ML_Agent_VehicleEnvironment_static_windows.zip?dl=0)
- Car Game Static Obs Mac [Link](https://www.dropbox.com/s/8gl0fa11rbwvqaz/ML_Agent_VehicleEnvironment_static_mac.zip?dl=0)
- Car Game Static Obs Linux [Link](https://www.dropbox.com/s/1ubddebgl11ggft/ML_Agent_VehicleEnvironment_static_linux.zip?dl=0)

---

### Flappy Bird Style Game

<img src="./Images/FlappyBird.png" width="500" alt="FlappyBird" />



This is similar with famous game Flappy Bird.

I implemented this game from [Unity Lecture](https://unity3d.com/kr/learn/tutorials/topics/2d-game-creation/project-goals?playlist=17093)

Yellow bird moves up and down. The bird has not to be collided with ground or columns. Also, if it goes above the screen, the game ends. 

```
The rules of the flappy bird are as follows.
+1 Reward
- Agent moves through the columns: reward

-1 Reward
- Agent collide with columns
- Agent collide with ground
- Agent moves above the screen

Terminal conditions
- It is same with the -1 reward condition
```



Download links of this environments are as follows.

- Flappy Bird Windows [Link](https://www.dropbox.com/s/724kc0i6ck1tpj6/ML_Agent_FlappyBird_Windows.zip?dl=0)
- Flappy Bird Mac [Link](https://www.dropbox.com/s/eajorh7d4sxix6q/ML_Agent_FlappyBird_MAC.zip?dl=0)
- Flappy Bird Linux [Link](https://www.dropbox.com/s/qiw8b6ts8vd6g1u/ML_Agent_FlappyBird_Linux.zip?dl=0)

---

### Pong

<img src="./Images/Pong_sample_img.PNG" width="500" alt="Pong" />



This is simple and popular environment for testing deep reinforcement learning algorithms.

Two bars have to hit the ball to win the game.  In my environment, left bar is `agent` and right bar is `enemy`. Enemy is invincible, so it can hit every ball.  In every episode, ball is fired in random direction.

```
The rules of the pong are as follows.
- Agent hits the ball: reward +1
- Agent misses the ball: reward -1

Terminal conditions
- Agent misses the ball
- Agent hit the ball 5 time in a row
```



Download links of this environments are as follows.

- Pong Windows [Link](https://www.dropbox.com/s/j7ib4k6f64gw1ft/ML_Agent_Pong_Windows.zip?dl=0)
- Pong Mac [Link](https://www.dropbox.com/s/8dci73a65wa8kuu/ML_Agent_Pong_Mac.zip?dl=0)
- Pong Linux [Link](https://www.dropbox.com/s/ren5lob8877iuby/ML_Agent_Pong_Linux.zip?dl=0)


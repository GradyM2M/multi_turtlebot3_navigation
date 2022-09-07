# multi_turtlebot3_navigation

#### 介绍
该功能包与[multi_rrt_exploration](https://github.com/GradyM2M/multi_rrt_exploration)配合使用，move_base与gmapping已经配置完毕。其中，算法验证平台采用3台TurtleBot3机器人设计与开发。结果表明，无论在仿真还是样机实验中，基于RRT-GFE的多机器人协同探索算法均能取得更加省时高效的探索效果。

#### 软件依赖
所需依赖如下：
1. 地图融合：[m-explore](https://github.com/hrnr/m-explore)
2. 探索插件：[frontier_exploration](https://github.com/paulbovbel/frontier_exploration)
3. 机器人模型：[turtlebot3](https://github.com/ROBOTIS-GIT/turtlebot3)
4. [turtlebot3_msgs](https://github.com/ROBOTIS-GIT/turtlebot3_msgs)
5. [Gmapping](https://github.com/ros-perception/openslam_gmapping)  

#### 使用说明

运行：  
```sh
$ roslaunch multi_turtlebot3_navigation multi_turtlebot3_gazebo.launch
$ roslaunch multi_turtlebot3_navigation move_base_three.launch
$ roslaunch multi_turtlebot3_navigation navigation_three.launch
```

rrt_exploration:
```sh 
$ roslaunch multi_turtlebot3_navigation exploring_three.launch
$ roslaunch multi_rrt_exploration rrt_three_robots.launch
```

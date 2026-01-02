# stanley_ros_demo
该项目基于 https://github.com/Raiden49/stanley_controller 跑通了Stanley路径跟踪的仿真实现，

![2](src/stanley_controller/docs/2.gif)

## 如何运行

新开一个终端，为终端1
- 进入目录, `cd ../stanley_ros_demo`
- 初始化工作空间, `catkin_make`
- 编译 Stanley Controller
  - `cd ../stanley_ros_demo/src/stanley_controller`
  - `mkdir build`
  - `cd build`
  - `cmake ..`
  - `make`

新开一个终端，为终端2
- 进入目录, `cd ../stanley_ros_demo`
- `source ./devel/setup.bash`
- 启动turtlebot3节点, `roslaunch turtlebot3_fake turtlebot3_fake.launch`

回到终端1
- 进入目录, `cd ../stanley_ros_demo`
- `source ./devel/setup.bash`
- 启动 stanley controller 节点, `roslaunch stanley_controller stanley_controller.launch`

![2](src/stanley_controller/docs/1.gif)
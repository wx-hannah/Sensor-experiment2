# Sensor-experiment2
Sensor , the second experiment on class on 3.14


# 进入工作空间
cd wx_ros_class_ws

source devel/setup.bash

cd src

# 进入功能包
roscd my_package_pkg
# 新终端 启动硬件
roslaunch upros_bringup bringup_w2a.launch

# 1、启动碰撞传感器避障
rosrun my_package_pkg ros_bump_node

# 2、启动超声波避障
rosrun my_package_pkg ros_sonic_node

# 3、启动imu转弯
rosrun my_package_pkg ros_imu_node

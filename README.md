![image](https://github.com/Robotics-Aerial-Robots/Homework6/blob/master/Figures/LOGO%20%E4%B8%AD%E8%8B%B1%E6%96%87%E6%A9%AB.png)
# 109 年度 機器人學：多軸旋翼機

# Final-project

### QP part
### Quadratic Programming
Then we provide the two examples, one is test-example which can produce  the shape of "eight" trajectory(as bleow image). The shape of "eight" trajectory is the final project path. Another is husky-path example which can provide you how to trace your desired path and trajectory path(line 201-271).\
`trajectory.png`

中文：我們提供了兩個範例,一個是test-example,他可以提供一個繞八的軌跡(如下圖),也是此次期末專題的軌跡. 另一個是husky-path,他提供你簡單參考範例,利用PID控制來追上你的軌跡,你可以參考此範例的201-207行

![image](https://github.com/Robotics-Aerial-Robots/Final_project/blob/master/photo/trajectory.png)

### Requirements
It is necessary to install python-cvxopt lib and eigen lib. 

```
sudo apt-get install libeigen3-dev
sudo apt-get install python-cvxopt

```

### How to use?
1. Cmake
```
cd qpc 
mkdir build && cd build
cmake ..
make
./cvxqp
```

2. rospackage
```
clone folder "qptrajectory_ros" to ~/catkin_ws/src

cd ~catkin_ws

catkin_make

rosrun qptrajectory qptest

rqt_plot

```

If the above installation is unsuccessful, or if you have doubts about the use of examples, please contact the teaching assistants.
中文：上述如有安裝不成功,或是有範例上使用疑慮請與助教們聯絡

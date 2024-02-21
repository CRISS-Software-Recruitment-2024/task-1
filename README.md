# task-1

IMPORTANT NOTE: The tutorial at https://github.com/CRISS-Robotics/learn-ros is a pre-requisite for this task. If you haven't completed the tutorial, do that first.

Task 1: Publisher and Subscriber in ROS

When you run ```rostopic list``` while the robot simulation is running, you see an output similar to the following:

![image](https://github.com/CRISS-Software-Recruitment-2024/task-1/assets/130831099/b5a3f9e9-ed52-4727-863f-64e59531a83b)

Here the topic ```/robot_base_velocity_controller/odom``` publishes the odometry of the robot (i.e. the position, orientation, and linear and angular velocities).

Try running the following to see what is being published to this topic
```
rostopic echo /robot_base_velocity_controller/odom
```

Your task is to create a subscriber that takes the position (x, y, and z values) of the robot from this topic. You then have to use these values to calculate the distance of the robot from the origin. Then, using a publisher, publish that value to a new topic.

You need to upload the Python file(s) here as your submission.

![rosgraph](https://user-images.githubusercontent.com/73032093/115158081-febaab00-a07b-11eb-855d-b8fdd51d1f2f.png)
Research_Track_first assignment  by Vikass Reddy 

this assignment is going to control holonomic robot in a 2d space.
### A brief explanation of the Algorithm
1. The robot asks for a random target, with both coordinates in the interval (-6.0, 6.0).
2. The robot reaches the target.
3. it will go to step 1.


### content of package
node
First node: (assignment1)

ROS publisher: publishing the robot speed
ROS client: receiving a random target

Second node: (project1)
ROS server: Service Server replys to the client with a random target

Costum service
Random_Target service: return two random positions between [-6.0, 6.0]

How to run the code
After git clone, move repository to /home/
Add the line 'source /home/my_ros_ws/devel/setup.bash' in your .bashrc file.

Change the directory to the workspace /home/my_ros_ws/
Build the packages 'catkin_make'

Refresh 'rospack profile'
Run the simulator

$ roscore &
$ rosrun stage_ros stageros $(rospack find assignment1)/world/exercise.world

Run the service node
$ rosrun project1 project1

Run the First node
$ rosrun assignment1 assignment1

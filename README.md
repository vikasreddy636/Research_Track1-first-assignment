
Research_Track_first assignment   (Ginne Vikas Reddy)(matricola 5061211)
The assignment requires controlling a holonomic robot in a 2d space with a simple 2d simulator

### A brief explanation of the Algorithm
1. The robot asks for a random target, with both coordinates in the interval (-6.0, 6.0).
2. The robot reaches the target.
3. it will go to step 1.


### content of package
node
First node: (assignment1)

ROS publisher: publishing the robot speed
ROS subscribe: subscribe for robot position
ROS client: receiving a random target

Second node: (node1)
ROS server: Service Server replys to the client with a random target


## How to run the code
git clone the package

`https://github.com/vikasreddy636/Research_Track1-first-assignment.git`

create a workspace in root repositories

`mkdir "name of the workspace" `

move the git package to the src folder of that workspace

Build the package

`catkin_make`

Refresh the workspace using

`rospack profile`

##Run the simulator

To start rosmaster

 'roscore'
 
 To launch the simulator
 
 'rosrun stage_ros stageros $(rospack find assignment1)/world/exercise.world'

Run the service node
'rosrun node1 node1'

Run the First node
'rosrun assignment1 assignment1'

## Software architecture
![rosgraph](https://user-images.githubusercontent.com/73032093/115158081-febaab00-a07b-11eb-855d-b8fdd51d1f2f.png)

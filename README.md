# Home-Service-Robot
A home service robot that will autonomously map an environment and navigate to pickup and deliver objects
The packages used in this project includes ros official packages and my own packages.

ros packages include
gmapping: This package can be used to perform SLAM and build a map of the environment with a robot equipped with laser range finder sensors or RGB-D cameras.
turtlebot_teleop: This package can be used to manually control a robot using keyboard commands.
turtlebot_rviz_launchers: This package can be used to load a preconfigured rviz workspace.
turtlebot_gazebo: This package can be used to deploy a turtlebot in a gazebo environment by linking the world file to it.

my own packages include 
pick_objects: The pick_objects node in this package is able to navigate the robot to a pick-up zone, wait for a while, and then navigate the robot to a drop-off zone.
add_markers: The add_markers node in this package is able to draw a marker in any location in the map. It also subscribes to the robot odom topic so the marker can be drawn (added) or erased (deleted) depending on the position and orientation of the robot.

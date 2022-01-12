cmake_minimum_required(VERSION 3.0.2)
project(ackermann_qt)

find_package(catkin REQUIRED COMPONENTS
  ackermann_msgs
  dynamic_reconfigure
  rospy
)

generate_dynamic_reconfigure_options(
  cfg/QTeleop.cfg
)

catkin_package(
#  INCLUDE_DIRS include
#  LIBRARIES ackermann_qt
#  CATKIN_DEPENDS ackermann_msgs dynamic_reconfigure rospy
#  DEPENDS system_lib
)

include_directories(
# include
  ${catkin_INCLUDE_DIRS}
)

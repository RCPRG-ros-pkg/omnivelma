cmake_minimum_required(VERSION 2.8.3)
project(omnivelma_msgs)

find_package(catkin REQUIRED COMPONENTS
  std_msgs
  geometry_msgs
  message_generation
  message_runtime
)

add_message_files(
	FILES
	Vels.msg
	Encoders.msg
	EncodersStamped.msg
	Relative.msg
	RelativeStamped.msg
)

add_service_files(
	FILES
	SetFriction.srv
	SetInertia.srv
	SetVelocity.srv
)

generate_messages(
	DEPENDENCIES
	std_msgs
	geometry_msgs
)


catkin_package(
	CATKIN_DEPENDS 
	std_msgs
	geometry_msgs
)

find_package(std_msgs REQUIRED)
find_package(geometry_msgs REQUIRED)
include_directories(${std_msgs_INCLUDE_DIRS})
include_directories(${geometry_msgs_INCLUDE_DIRS})

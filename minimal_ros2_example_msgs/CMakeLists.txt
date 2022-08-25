cmake_minimum_required(VERSION 3.8)
project(minimal_ros2_example_msgs)

find_package(ament_cmake REQUIRED)
find_package(rosidl_default_generators REQUIRED)

rosidl_generate_interfaces(${PROJECT_NAME} "msg/Colour.msg" DEPENDENCIES)

ament_package()

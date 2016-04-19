cmake_minimum_required(VERSION 2.4.6)
project(ardrone_joystick)

find_package(catkin REQUIRED COMPONENTS
  sensor_msgs
  geometry_msgs
  roscpp
  std_srvs
)

catkin_package(
  DEPENDS sensor_msgs geometry_msgs roscpp std_srvs
)

#set the default path for built executables to the "bin" directory
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
#set the default path for built libraries to the "lib" directory
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)


add_executable(ardrone_joystick src/main.cpp)
target_link_libraries(ardrone_joystick ${catkin_LIBRARIES})

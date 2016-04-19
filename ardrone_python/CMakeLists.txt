cmake_minimum_required(VERSION 2.4.6)
project(ardrone_python)

find_package(catkin REQUIRED COMPONENTS rospy)

catkin_package()

#set the default path for built executables to the "bin" directory
set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
#set the default path for built libraries to the "lib" directory
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

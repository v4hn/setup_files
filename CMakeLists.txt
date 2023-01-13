cmake_minimum_required(VERSION 3.0.2)
project(setup_files)

find_package(catkin QUIET)

catkin_package()

# TODO(v4hn): generate files dynamically
# this is currently hard-coded to /opt/ros/debian/
if(NOT CATKIN_DEVEL_PREFIX)
  install(DIRECTORY files/ DESTINATION ${CMAKE_INSTALL_PREFIX})
endif()

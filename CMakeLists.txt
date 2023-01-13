cmake_minimum_required(VERSION 3.0.2)
project(setup_files)

find_package(catkin QUIET)

catkin_package()

if(NOT CATKIN_DEVEL_PREFIX)
  install(DIRECTORY files/ DESTINATION ${CMAKE_INSTALL_PREFIX})
endif()

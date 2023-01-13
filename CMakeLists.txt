cmake_minimum_required(VERSION 3.0.2)
project(setup_files)

install(DIRECTORY files/ DESTINATION ${CMAKE_INSTALL_PREFIX})

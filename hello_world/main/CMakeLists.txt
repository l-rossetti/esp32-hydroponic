# The following lines of boilerplate have to be in your project's
# CMakeLists in this exact order for cmake to work correctly
#cmake_minimum_required(VERSION 3.16)

#include($ENV{IDF_PATH}/tools/cmake/project.cmake)
#project(hello_world)
idf_component_register(SRCS "hello_world_main.c"
                    INCLUDE_DIRS "")
cmake_minimum_required(VERSION 3.4)
project(imagemagick_cpp)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_SOURCE_DIR}/cmake/modules/")

find_package(ImageMagick REQUIRED)

set(SOURCE_FILES main.cpp)
add_executable(imagemagick_cpp ${SOURCE_FILES})
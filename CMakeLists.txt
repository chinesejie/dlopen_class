cmake_minimum_required(VERSION 3.5)
project(dlopen_class)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -g -ldl -std=c++11")

file(GLOB sources "${CMAKE_CURRENT_SOURCE_DIR}/main.cpp")
# do not include polygon.cpp 

add_executable(dlopen_clazz ${sources})

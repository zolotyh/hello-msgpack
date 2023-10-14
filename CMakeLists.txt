cmake_minimum_required(VERSION 3.15)
project(msgpack_example)

message("Building with CMake version: ${CMAKE_VERSION}")
message("Building project name: ${PROJECT_NAME}")

find_package(msgpack REQUIRED)

add_executable(${PROJECT_NAME} src/main.cpp)
target_link_libraries(${PROJECT_NAME} msgpackc-cxx)

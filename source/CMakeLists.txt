cmake_minimum_required(VERSION 3.27)
project(dx11play)

set(CMAKE_CXX_STANDARD 17)

add_executable(dx11play main.cpp)

find_package(SDL REQUIRED)

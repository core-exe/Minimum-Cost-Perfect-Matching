cmake_minimum_required(VERSION 3.10)

project(minimum_cost_perfect_matching)

set( CMAKE_EXPORT_COMPILE_COMMANDS ON )

set(CMAKE_C_STANDARD 11)
set(CMAKE_CXX_STANDARD 17)

add_library(minimum_cost_perfect_matching STATIC
    BinaryHeap.h
    BinaryHeap.cpp
    Globals.h
    Graph.cpp
    Graph.h
    Matching.cpp
    Matching.h
)

target_include_directories(minimum_cost_perfect_matching PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}")
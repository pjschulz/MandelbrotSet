cmake_minimum_required(VERSION 3.8)
project(MandelbrotSet)

set(CMAKE_C_STANDARD 11)

set(SOURCE_FILES main.c)
add_executable(MandelbrotSet ${SOURCE_FILES})

find_library(M_LIB m)
target_link_libraries(MandelbrotSet ${M_LIB})

find_package(OpenMP)
set (CMAKE_C_FLAGS "${CMAKE_C_FLAGS} ${OpenMP_C_FLAGS}")
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${OpenMP_CXX_FLAGS}")
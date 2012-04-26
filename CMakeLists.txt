project(Hello-World)
cmake_minimum_required(VERSION 2.8 FATAL_ERROR)

set(SOURCES main.cpp)

add_executable(Hello ${SOURCES})

if(CMAKE_COMPILER_IS_GNUCXX)
    set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
endif()

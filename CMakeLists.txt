cmake_minimum_required(VERSION 3.22)

project(yen VERSION 0.1 DESCRIPTION "Command line tools manager" LANGUAGES CXX)

file(GLOB_RECURSE SOURCES src/*.cpp)

add_executable(${CMAKE_PROJECT_NAME} ${SOURCES})
set_property(TARGET ${CMAKE_PROJECT_NAME} PROPERTY CXX_STANDARD 20)


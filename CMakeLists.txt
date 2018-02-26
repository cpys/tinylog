cmake_minimum_required(VERSION 3.5)
project(tinylog)

include_directories(${PROJECT_SOURCE_DIR}/src)

set(CMAKE_CXX_STANDARD 11)

include_directories(headers)

set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/output)

add_library(tinylog SHARED src/Logger.cpp)

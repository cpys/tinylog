cmake_minimum_required(VERSION 3.5)
project(tinylog)

set(CMAKE_CXX_STANDARD 11)

include_directories(headers)

set(EXECUTABLE_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/bin)
set(LIBRARY_OUTPUT_PATH ${PROJECT_SOURCE_DIR}/lib)

add_library(tinylog SHARED src/Logger.cpp)
add_executable(tinylogtest src/Logger.cpp src/logTest.cpp)
cmake_minimum_required(VERSION 3.12)
project(aStar)
find_package(OpenCV REQUIRED)

set(CMAKE_CXX_STANDARD 14)

add_executable(aStar main.cpp aStarSearch.cpp aStarSearch.h)
target_link_libraries(aStar ${OpenCV_LIBS})
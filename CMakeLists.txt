cmake_minimum_required(VERSION 3.13)

project(Optical Flow)
set(CMAKE_CXX_STANDARD 11)            # Enable c++11 standard

find_package( OpenCV REQUIRED )
include_directories( ${OpenCV_INCLUDE_DIRS} )

add_executable(opt_flow opt_flow.cpp) 
target_link_libraries( opt_flow ${OpenCV_LIBS} )

add_executable(opt_tracking opt_tracking.cpp) 
target_link_libraries( opt_tracking ${OpenCV_LIBS} )

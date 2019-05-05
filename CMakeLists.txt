cmake_minimum_required(VERSION 2.6)
project(parkinglinedetection)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11")
find_package( OpenCV REQUIRED )

add_executable(parkinglinedetection main.cpp)

target_link_libraries( parkinglinedetection ${OpenCV_LIBS} )

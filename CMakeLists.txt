cmake_minimum_required(VERSION 2.8)
project( BAvisSfM )
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fopenmp -O4")
find_package( OpenCV REQUIRED )
add_executable( BAvisSfM main.cpp BAutil.cpp)
target_link_libraries( BAvisSfM ${OpenCV_LIBS})

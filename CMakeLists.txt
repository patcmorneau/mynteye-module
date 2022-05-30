cmake_minimum_required(VERSION 3.0)

project(get_depth)

find_package(OpenCV 4.2 REQUIRED)
find_package(mynteye REQUIRED)
add_executable(getdepth get_depth.cpp)
target_link_libraries(getdepth mynteye ${OpenCV_LIBS})




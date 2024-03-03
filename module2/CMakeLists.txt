
cmake_minimum_required(VERSION 3.0.0)
project("Calculator Project" VERSION 1.0.0)

add_library(mathlibrary 
	addition.cpp
	division.cpp)

add_library(outputresult print_result.cpp)

add_executable(Calculator main.cpp)
add_executable(App main.cpp)


target_link_libraries(Calculator PRIVATE mathlibrary outputresult)
target_link_libraries(App PRIVATE mathlibrary outputresult)


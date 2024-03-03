
cmake_minimum_required(VERSION 3.0.0)
project("Calculator Project" VERSION 1.0.0)


add_subdirectory(maths)
add_subdirectory(print)

add_executable(Calculator main.cpp)

target_link_libraries("Calculator" PRIVATE mathlibrary outputresult)

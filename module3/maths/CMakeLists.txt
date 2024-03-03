

add_library(mathlibrary src/addition.cpp src/division.cpp)

target_include_directories(
   mathlibrary
   PUBLIC
   include)
   

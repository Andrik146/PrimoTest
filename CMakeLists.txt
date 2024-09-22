cmake_minimum_required(VERSION 3.29)
project(ProgettoGit)

set(CMAKE_CXX_STANDARD 14)

add_subdirectory(src)
include_directories(.)
add_library(matematica STATIC src/matematica.cpp)

add_executable(ProgettoGit main.cpp)
target_link_libraries(ProgettoGit matematica)

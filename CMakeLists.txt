cmake_minimum_required(VERSION 3.24)
project(sparse)

set(CMAKE_CXX_STANDARD 20)

add_executable(sparse main.cpp)


set(GLFW_BUILD_DOCS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_TESTS OFF CACHE BOOL "" FORCE)
set(GLFW_BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)
add_subdirectory(vendor/glfw)
target_link_libraries(sparse glfw)
#include_directories(vendor/glfw/include)


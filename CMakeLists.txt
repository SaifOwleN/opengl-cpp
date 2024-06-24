cmake_minimum_required(VERSION 3.10)

project(xddMORS)

find_package(fmt REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
find_package(OpenGL REQUIRED)
find_package(GLEW REQUIRED)

add_executable(${PROJECT_NAME} main.cpp)

target_link_libraries(${PROJECT_NAME} PUBLIC fmt::fmt glfw OpenGL::GL GLEW::GLEW)

# add_library(MathFunctions MathFunctions.cxx mysqrt.cxx)

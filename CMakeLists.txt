# Set the minimum version of CMake that can be used
# To find the cmake version run
# $ cmake --version
cmake_minimum_required(VERSION 3.5)

find_package(Matplot++ REQUIRED)

# Set the project name
project (main)

# Create an executable target
add_executable(${PROJECT_NAME} main.cpp)
target_link_libraries(${PROJECT_NAME} PUBLIC Matplot++::matplot)
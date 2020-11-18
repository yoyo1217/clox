cmake_minimum_required(VERSION 3.13)  # CMake version check
project(clox)               # Create project "simple_example"
set(CMAKE_CXX_STANDARD 14)            # Enable c++14 standard

# Add main.cpp file of project root directory as source file
set(SOURCE_FILES main.cpp)


FILE(GLOB my_c_sources *.c)
# Add executable target with source files listed in SOURCE_FILES variable
#add_executable(myProgram main.c chunk.c debug.c memory.c value.c vm.c scanner.c compiler.c)
add_executable(myProgram ${my_c_sources})
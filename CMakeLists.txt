cmake_minimum_required(VERSION 3.10)  # CMake version check
project(comp30023-2020-project1)               # Create project "simple_example"
set(CMAKE_CXX_STANDARD 11)            # Enable c++14 standard
set(CMAKE_CXX_FLAGS "-O3 -Wall -Wextra")

# Add executable target with source files listed in SOURCE_FILES variable
FILE(GLOB_RECURSE SOURCE_FILE src/*.c lib/*.c)
add_executable(crawler ${SOURCE_FILE} src/url.c src/url.h src/collection.c)
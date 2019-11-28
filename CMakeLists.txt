cmake_minimum_required(VERSION 3.1)
project(TheGame)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(CMAKE_BUILD_TYPE Release)

set(CMAKE_CXX_FLAGS "-Wall -Wextra")
set(CMAKE_CXX_FLAGS_RELEASE "-O3")

add_executable(TheGame src/main.cpp)
target_include_directories(TheGame PRIVATE src)
target_link_libraries(TheGame PRIVATE sfml-graphics sfml-window sfml-system)

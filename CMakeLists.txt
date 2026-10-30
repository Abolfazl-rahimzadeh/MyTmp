cmake_minimum_required(VERSION 3.25)

project(MyTmp
    VERSION 0.1.0
    DESCRIPTION "A temporary directory management utility"
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(mytmp
    src/main.cpp
)

target_compile_options(mytmp PRIVATE
    -Wall
    -Wextra
    -Wpedantic
    -Wconversion
    -Wshadow
)

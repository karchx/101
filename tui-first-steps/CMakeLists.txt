cmake_minimum_required(VERSION 3.10)

project(hello VERSION "0.0.1" LANGUAGES CXX)

# Let's stick to modern C++17
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

set(CMAKE_EXPORT_COMPILE_COMMANDS ON)

set(lib_SRC src/lib/fontconfig.cpp src/lib/fontconfig.h)

add_executable(tui src/app/main.cpp ${lib_SRC})

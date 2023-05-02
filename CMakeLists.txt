cmake_minimum_required(VERSION 3.10)

# Set c++ version
set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

# languages
project(day14new LANGUAGES CXX)

# 子项目（顺序无关紧要）
add_subdirectory(WebServer)


# HTTP

# Release
if(NOT CMAKE_BUILD_TYPE)
    set(CMAKE_BUILD_TYPE "Release")
endif()
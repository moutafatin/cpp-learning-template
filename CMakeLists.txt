cmake_minimum_required(VERSION 3.27)


project(app VERSION 0.1.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 20)

set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -pedantic-errors -Wall -Weffc++ -Wextra -Wconversion -Wsign-conversion -Werror -std=c++20")

file(GLOB SOURCES src/*.cpp)

add_executable(app ${SOURCES})

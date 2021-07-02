cmake_minimum_required(VERSION 3.17)
project(prova)

set(CMAKE_CXX_STANDARD 14)



find_package(Curses REQUIRED)
include_directories(${CURSES_INCLUDE_DIR})
add_executable(prova main.cpp)
target_link_libraries(prova ${CURSES_LIBRARIES})
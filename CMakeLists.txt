cmake_minimum_required(VERSION 3.5.0)
project(pathFinding VERSION 0.1.0 LANGUAGES C CXX)

set(CMAKE_CXX_STANDARD 14)

include_directories(src/include)
file(GLOB SOURCES "src/*.cpp")
add_executable(pathFinding ${SOURCES})
target_link_libraries(pathFinding PRIVATE sfml-graphics sfml-window sfml-system)


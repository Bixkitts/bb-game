cmake_minimum_required(VERSION 3.0)

project(bb-game-server)

include_directories(src)
file(GLOB_RECURSE SOURCES "src/*.cpp")
add_executable(bb-game-server ${SOURCES})

target_link_options(bb-game-server PRIVATE -pthread)
#target_compile_options(bb-game-server PRIVATE -o1)

cmake_minimum_required(VERSION 4.3)
project(daur)

set(CMAKE_CXX_STANDARD 26)

file(GLOB_RECURSE daur_sources
    ${CMAKE_SOURCE_DIR}/src/**.cpp
    ${CMAKE_SOURCE_DIR}/src/**.hpp
)
add_executable(daur ${daur_sources})
target_include_directories(daur PRIVATE src/)
cmake_minimum_required(VERSION 2.8)
project(dfa)

set(OUTPUTNAME dfa.out)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -O3 -std=c++11")

aux_source_directory(. DIR_SRCS)

add_executable(${OUTPUTNAME} ${DIR_SRCS})

target_link_libraries(${OUTPUTNAME} pthread)

cmake_minimum_required(VERSION 3.22)

project(example C)

set(CMAKE_C_STANDARD 99)

add_executable(example main.c)

find_package(GSL REQUIRED)

target_link_libraries(example GSL::gsl GSL::gslcblas)
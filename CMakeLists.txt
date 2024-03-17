cmake_minimum_required(VERSION 3.22 FATAL_ERROR)

project(
    "First_CMake_Project"
    VERSION 1.0.0
    DESCRIPTION "CMake C Project template for Operative Systems II"
    LANGUAGES C
    #AUTHOR "Landaeta Ezequiel Matias"
)

set(CMAKE_C_STANDARD 17)

include_directories(include)

file(GLOB_RECURSE SOURCES "src/*.c")

#set(CMAKE_C_FLAGS)

add_executable(${PROJECT_NAME} ${SOURCES})
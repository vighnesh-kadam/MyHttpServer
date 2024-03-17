cmake_minimum_required (VERSION 3.5)

project (test1)

set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -Wall -std=c++14")
set (source_dir "${PROJECT_SOURCE_DIR}/src/")

file (GLOB_RECURSE source_files "${source_dir}/*.cpp" "${source_dir}/*.hpp")

add_executable (test1 ${source_files})



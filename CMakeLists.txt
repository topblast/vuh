cmake_minimum_required(VERSION 3.8)
project(vuh VERSION 1.1.1)

option(VUH_BUILD_BENCHMARKS "Build benchmarks for vuh library" OFF)
option(VUH_BUILD_DOCS "Build doxygen documentation for vuh" ON)
option(VUH_BUILD_EXAMPLES "Build examples of using vuh" ON)
option(VUH_BUILD_TESTS "Build tests for vuh library" ON)

set(CMAKE_CXX_STANDARD 14)
list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/config)
enable_testing()

add_subdirectory(doc)
add_subdirectory(src)
add_subdirectory(test)

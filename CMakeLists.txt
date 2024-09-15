cmake_minimum_required(VERSION 3.22)
project(cpp_template_workspace VERSION 1.0 LANGUAGES CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Conan setup
include(${CMAKE_BINARY_DIR}/conan.cmake)
conan_cmake_configure(REQUIRES gtest/1.11.0 GENERATORS cmake)
conan_cmake_install(PATH_OR_REFERENCE . BUILD missing)

# Add executable for the main application
add_executable(cpp_template_workspace src/main.cpp)

# Add subdirectory for tests
add_subdirectory(tests)

cmake_minimum_required(VERSION 3.22)
project(cpp_template_workspace VERSION 1.0 LANGUAGES CXX)

# Set C++ standard
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Add executable for the main application
add_executable(cpp_template_workspace src/main.cpp)

# Enable testing
enable_testing()

# Add subdirectory for tests
add_subdirectory(tests)

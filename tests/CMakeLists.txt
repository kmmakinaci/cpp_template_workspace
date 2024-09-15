# Minimum CMake version required
cmake_minimum_required(VERSION 3.22)

# Project name
project(tests LANGUAGES CXX)

# GoogleTest setup
find_package(GTest REQUIRED)

# Add the test executable
add_executable(test_main test_main.cpp)
target_link_libraries(test_main PRIVATE GTest::gtest GTest::gtest_main)

# Add test to CTest
add_test(NAME MyTests COMMAND test_main)

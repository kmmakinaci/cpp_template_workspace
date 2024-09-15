# Tests for the project
add_executable(test_main test_main.cpp)
target_link_libraries(test_main PRIVATE ${CONAN_LIBS})

add_test(NAME MyTests COMMAND test_main)

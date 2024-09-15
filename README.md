# My C++ Project

## Project Overview
This project template uses CMake and Conan for package management and Google Test for unit testing.

```bash
my_cpp_project/
├── build/               # For out-of-source builds
├── include/
│   └── my_project.h
├── src/
│   └── main.cpp
├── tests/
│   └── test_main.cpp
├── .clang-format
├── .gitignore
├── .pre-commit-config.yaml
├── conanfile.txt
├── CMakeLists.txt
└── README.md
```

## Build Instructions

1. **Install Conan**:
   [Conan](https://conan.io/) must be installed on your system.

2. **Build the Project**:
   ```bash
   mkdir build
   cd build
   conan install ..
   cmake ..
   cmake --build .
   ```
3. **Run Tests:**
   ```bash
   ctest
   ```
4. **Dependencies**
* CMake
* Conan
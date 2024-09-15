# My C++ Project

## Project Overview
This project template uses CMake and Google Test for unit testing.

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
├── CMakeLists.txt
└── README.md

## Build Instructions

1. **Dependencies**
* CMake
* GoogleTest:
Make sure you have Google Test installed on your system. On Ubuntu, you can install it using:

```bash
sudo apt-get install libgtest-dev
```
You might need to build Google Test from source if the package doesn't include pre-built libraries:
```bash
cd /usr/src/googletest
sudo cmake CMakeLists.txt
sudo make
sudo cp *.a /usr/lib
```

2. **Build the Project**:
Create a build directory:
```bash
mkdir build
cd build
```

Configure the project:
```bash
cmake -DCMAKE_BUILD_TYPE=Release ..
```

Build the project:
```bash
cmake --build .
```

3. **Run Program & Tests:**
```bash
~/repos/workspace-cpp/cpp_template_workspace/build$ ./cpp_template_workspace
~/repos/workspace-cpp/cpp_template_workspace/build$ ctest-V
```

PS: See the notes regarding [naming conventions](https://github.com/kmmakinaci/MyNoteBook/blob/master/NamingConventionsInSW.md) in software development.
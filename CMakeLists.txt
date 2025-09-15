cmake_minimum_required(VERSION 3.10)
project(MyLang)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Include directories
include_directories(include src)

# Source files
set(SOURCES
    src/lexer.cpp
    src/parser.cpp
    src/semantic.cpp
    src/vm.cpp
    src/bytecode.cpp
    src/compiler.cpp
    src/repl.cpp
    src/builtins.cpp
    src/main.cpp
)

# Executable for interpreter and compiler
add_executable(myinterpreter ${SOURCES})

# Optionally, you can add tests and other targets here

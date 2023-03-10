# Declare the minimum CMake version required: this allows safely
# using functionality up to the specified version, without encurring
# in puzzling error messages.
# NB: in practice, it is ok to choose an agreed upon version even if
# its latest functionalities are not used.
cmake_minimum_required(VERSION 3.14)

# Specify a project name.
# This is generally useful, and required for interoperability.
# Optional options include 'VERSION', 'DESCRIPTION', 'LANGUAGES'
# and 'HOMEPAGE_URL'
project(cmake_tutorial VERSION 1.0
    DESCRIPTION "A tutorial on how to use CMake for C++ projects")

# Supposing you are building an application, specify an executable:
# its target name and its source file (containing the 'main' function).
# NB: 'add_executable' may be invoked multiple times, each time
# declaring a different executable associated to a unique target name.
add_executable(tutorial tutorial.m.cpp)
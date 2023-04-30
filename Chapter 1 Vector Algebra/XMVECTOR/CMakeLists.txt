cmake_minimum_required(VERSION 3.25)
project(XMVECTOR)

set(CMAKE_CXX_STANDARD 14)

add_executable(XMVECTOR
        InitFunctions.cpp
        tol.cpp
        VectorOps.cpp
        xmvec3.cpp)

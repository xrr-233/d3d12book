cmake_minimum_required(VERSION 3.25)
project(TexColumns)

set(CMAKE_CXX_STANDARD 14)
set(D3D_APP_SRC ../../Common/d3dApp.cpp)
set(D3D_UTIL_SRC ../../Common/d3dUtil.cpp)
set(GAME_TIMER_SRC ../../Common/GameTimer.cpp)
set(DDS_TEXTURE_LOADER_SRC ../../Common/DDSTextureLoader.cpp)
set(MATH_HELPER_SRC ../../Common/MathHelper.cpp)
set(GEOMETRY_GENERATOR_SRC ../../Common/GeometryGenerator.cpp)

add_executable(TexColumns WIN32
        FrameResource.cpp
        TexColumnsApp.cpp
        ${D3D_APP_SRC}
        ${D3D_UTIL_SRC}
        ${GAME_TIMER_SRC}
        ${DDS_TEXTURE_LOADER_SRC}
        ${MATH_HELPER_SRC}
        ${GEOMETRY_GENERATOR_SRC})
add_definitions(-DUNICODE)

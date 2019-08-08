cmake_minimum_required(VERSION 2.8.0)
project(SilentTextEditor)


SET(SOURCE
    src/main.cpp
    src/editor.cpp
)

SET(HEADERS
    include/editor.hpp
)

add_executable(
    SilentTextEditor
    ${SOURCE}
    ${HEADERS}
)

target_include_directories(
    SilentTextEditor PUBLIC "${CMAKE_CURRENT_SOURCE_DIR}/include"
)
cmake_minimum_required(VERSION 3.21)

project(STB
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_library(STB INTERFACE)

target_include_directories(
    STB INTERFACE ${CMAKE_CURRENT_SOURCE_DIR}/includes/
)

add_library(razer::stb ALIAS STB)

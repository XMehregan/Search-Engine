cmake_minimum_required(VERSION 3.16)

project(MiniSearchEngine
    VERSION 0.1.0
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_CXX_EXTENSIONS OFF)

add_executable(mini_search_engine
    src/main.cpp
)

if(CMAKE_CXX_COMPILER_ID MATCHES "GNU|Clang")
    target_compile_options(mini_search_engine PRIVATE
        -Wall
        -Wextra
        -Wpedantic
    )
endif()
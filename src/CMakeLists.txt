cmake_minimum_required(VERSION 3.15)
project(AutoPlay)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -fPIC")

add_library(AutoPlay SHARED src/main.cpp)

target_include_directories(AutoPlay PRIVATE
    /path/to/scotland2/include
    /path/to/beatsaber-hook/include
)

target_link_libraries(AutoPlay PRIVATE
    # Add any required libraries here
)

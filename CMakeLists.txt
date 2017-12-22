cmake_minimum_required(VERSION 3.8)
project(gl-breakout)

add_subdirectory(libs/alexlib)

add_executable(gl-breakout "")
target_sources(gl-breakout PRIVATE
        # headers
        # sources
        src/main.cpp)
target_include_directories(gl-breakout PRIVATE
        include
        libs/alexlib/include)
target_link_libraries(gl-breakout PRIVATE alexlib)

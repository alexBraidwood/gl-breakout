cmake_minimum_required(VERSION 3.8)
project(gl-breakout)

set(CMAKE_CXX_STANDARD 17)

add_subdirectory(libs/alexlib)

add_executable(gl-breakout "")
target_sources(gl-breakout PRIVATE
        # headers
        # sources
        src/main.cpp)
target_include_directories(gl-breakout PRIVATE
        include
        libs/alexlib/include
        libs/alexlib/external/glm)
target_link_libraries(gl-breakout PRIVATE alexlib)

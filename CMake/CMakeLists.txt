cmake_minimum_required(VERSION 3.5)

project(01.hello_world)

set(SOURCES
        ../HW2_VS_Project/Classes/hello_world.cpp
        ../HW2_VS_Project/Classes/example.cpp
        ../HW2_VS_Project/Classes/move_me_out.cpp
)

set(HEADERS
        ../HW2_VS_Project/Classes/example.h
        ../HW2_VS_Project/Classes/move_me_out.h
)

add_executable(hello_world
    ${SOURCES}
    ${HEADERS} 
)

set_target_properties(hello_world PROPERTIES
    CXX_STANDARD 17
    CXX_STANDARD_REQUIRED ON
)
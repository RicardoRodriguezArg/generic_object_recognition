cmake_minimum_required(VERSION 2.8)

project(object_processor)
find_package( Threads )
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}  -std=c++14 -o1")
include_directories(./src/definitions)
set(SOURCE_FILES



        )

add_executable (${PROJECT_NAME} main.cpp ${SOURCE_FILES} )
target_link_libraries ( ${PROJECT_NAME} ${CMAKE_THREAD_LIBS_INIT})



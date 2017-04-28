cmake_minimum_required(VERSION 2.8)

project(GenericObjectRecognizer)
SET(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS}  -std=c++14 -o1")
find_package( Threads )
add_subdirectory ( ./src/object_processor )













set(SOURCE_FILES

        src/main.cpp
        )
add_executable(${PROJECT_NAME} ${SOURCE_FILES})
TARGET_LINK_LIBRARIES(${PROJECT_NAME} ${CMAKE_THREAD_LIBS_INIT} )

cmake_minimum_required(VERSION 3.0.0)
project(Example1 VERSION 0.1.0)

#set(headerFiles inc/XX)
set(SOURCES src/main.cpp)



set(CMAKE_ARCHIVE_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/lib)
set(CMAKE_RUNTIME_OUTPUT_DIRECTORY ${CMAKE_BINARY_DIR}/bin)


add_executable(${PROJECT_NAME} ${SOURCES})
target_include_directories(${PROJECT_NAME} PRIVATE inc)
set(CMAKE_BUILD_TYPE debug) 



cmake_minimum_required(VERSION 4.2)

project(ProjectName)

set(CMAKE_RUNTIME_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/$<CONFIGURATION>")
set(CMAKE_LIBRARY_OUTPUT_DIRECTORY "${CMAKE_BINARY_DIR}/$<CONFIGURATION>")

add_executable(ProjectName)

target_sources(ProjectName
  PRIVATE
   src/main.cpp
)

target_include_directories(ProjectName
   PRIVATE
   include)

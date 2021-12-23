cmake_minimum_required(VERSION 3.20)

# Make the project
set(TARGET "hello_world")
project(${TARGET})

# Add library example
#add_library(LogitechLEDLib STATIC IMPORTED)
#set_target_properties(LogitechLEDLib PROPERTIES
#  IMPORTED_LOCATION "${CMAKE_SOURCE_DIR}/lib/LogitechLEDLib.lib"
#  INTERFACE_INCLUDE_DIRECTORIES "${CMAKE_SOURCE_DIR}/include/LogitechLEDLib"
#)

# Build the executable
set(SOURCE_FILES hello_world.cpp)
add_executable(${TARGET} ${SOURCE_FILES})

# Link library example
#target_link_libraries(${TARGET} PUBLIC LogitechLEDLib)
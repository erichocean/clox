cmake_minimum_required(VERSION 3.0.0)
project(clox)

include(CTest)
enable_testing()

file(GLOB SOURCES *.c)

add_executable(clox ${SOURCES})

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

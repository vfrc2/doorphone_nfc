cmake_minimum_required(VERSION 3.1)

project(doorphone_nfc VERSION 0.1.0)

add_executable(doorphone_nfc src/main.cpp)

configure_file(src/version.h.in version.h)
include_directories(${CMAKE_CURRENT_BINARY_DIR})

target_link_libraries(doorphone_nfc nfc)
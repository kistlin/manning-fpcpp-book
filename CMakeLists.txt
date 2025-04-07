cmake_minimum_required(VERSION 3.10)

SET(CMAKE_CXX_STANDARD 17)
SET(CMAKE_CXX_STANDARD_REQUIRED ON)

project(FPCPP)

add_compile_definitions("ASIO_STANDALONE")

include_directories(BEFORE SYSTEM ${CMAKE_CURRENT_SOURCE_DIR}/3rd-party/ericniebler/range-v3/include)
include_directories(BEFORE SYSTEM ${CMAKE_CURRENT_SOURCE_DIR}/3rd-party/nlohmann/json/include)
include_directories(BEFORE SYSTEM ${CMAKE_CURRENT_SOURCE_DIR}/3rd-party/chriskohlhoff/asio/asio/include)

find_package(Catch2 3.8 REQUIRED HINTS ${CMAKE_CURRENT_SOURCE_DIR}/3rd-party/catchorg/Catch2)

set_property(GLOBAL PROPERTY USE_FOLDERS ON)

add_subdirectory(3rd-party/catchorg/Catch2)
include_directories(common)
add_subdirectory(chapter-01)
add_subdirectory(chapter-02)
add_subdirectory(chapter-03)
add_subdirectory(chapter-04)
#add_subdirectory(chapter-05)
add_subdirectory(chapter-06)
add_subdirectory(chapter-07)
#add_subdirectory(chapter-08)
add_subdirectory(chapter-09)
add_subdirectory(chapter-10)
add_subdirectory(chapter-11)
add_subdirectory(chapter-12)
add_subdirectory(chapter-13)

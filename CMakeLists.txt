cmake_minimum_required(VERSION 3.23)
project(Computer_Vision)

include(CTest)
enable_testing()

find_package(OpenCV REQUIRED)
include_directories( ${OpenCV_INCLUDE_DIRS} )

add_executable(Computer_Vision main.cpp)

target_link_libraries( Computer_Vision ${OpenCV_LIBS} )

set(CMAKE_CXX_STANDARD 23)


include(CPack)
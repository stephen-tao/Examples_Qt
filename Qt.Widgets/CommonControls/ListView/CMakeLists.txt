cmake_minimum_required(VERSION 3.1)

# Project
project(ListView)
find_package(Qt5Widgets CONFIG REQUIRED)

# Options
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)
set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

# Application
add_executable(ListView WIN32 MACOSX_BUNDLE src/ListView.cpp src/ListView.h)
target_link_libraries(ListView Qt5::Widgets)

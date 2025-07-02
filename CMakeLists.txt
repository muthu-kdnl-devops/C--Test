cmake_minimum_required(VERSION 3.10)

project(MyQtApp)

set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

find_package(Qt5 COMPONENTS Widgets REQUIRED)

add_executable(MyQtApp
    main.cpp
    MainWindow.cpp
    MainWindow.h
)

target_link_libraries(MyQtApp Qt5::Widgets)

cmake_minimum_required(VERSION 3.5)
project(sfml_test)

set(CMAKE_CXX_STANDARD 17)

find_package(SFML COMPONENTS graphics window system audio REQUIRED)

add_executable(sfml_test
    src/main.cpp
    src/mainwindow.cpp
    src/Enemy.cpp
    src/Map.cpp
    src/Game.cpp
    src/Config.cpp
    src/AssetManager.cpp
    src/Tower.cpp
    src/WaveManager.cpp
    src/SaveManager.cpp
)

target_link_libraries(sfml_test sfml-graphics sfml-window sfml-system sfml-audio)

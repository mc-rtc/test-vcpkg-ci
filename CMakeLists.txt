cmake_minimum_required(VERSION 3.1)

project(MyProject LANGUAGES CXX VERSION 1.0.0)

find_package(rbdyn REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PUBLIC RBDyn::RBDyn)

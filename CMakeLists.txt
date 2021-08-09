cmake_minimum_required(VERSION 3.1)

project(MyProject LANGUAGES CXX VERSION 1.0.0)

enable_testing()

find_package(SpaceVecAlg REQUIRED)

add_executable(main main.cpp)
target_link_libraries(main PUBLIC SpaceVecAlg::SpaceVecAlg)
install(TARGETS main DESTINATION bin)

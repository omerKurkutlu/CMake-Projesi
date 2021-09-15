cmake_minimum_required(VERSION 3.0.0)
project(Polonom VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(
    Polonom 
    ./src/main.cpp 
)

add_subdirectory(Student)

target_include_directories(${PROJECT_NAME} PUBLIC Student)
target_link_directories(${PROJECT_NAME} PUBLIC Student)
target_link_libraries(Polonom PUBLIC studentLib)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

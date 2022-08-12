cmake_minimum_required(VERSION 3.0.0)
project(Deneme VERSION 0.1.0)

include(CTest)
enable_testing()

add_executable(
    Deneme 
    ./src/main.cpp 
)

add_subdirectory(Student)

target_include_directories(${PROJECT_NAME} PUBLIC Student)
target_link_directories(${PROJECT_NAME} PUBLIC Student)
target_link_libraries(Deneme PUBLIC studentLib)

set(CPACK_PROJECT_NAME ${PROJECT_NAME})
set(CPACK_PROJECT_VERSION ${PROJECT_VERSION})
include(CPack)

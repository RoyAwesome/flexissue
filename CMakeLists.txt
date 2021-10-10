# CMakeList.txt : Top-level CMake project file, do global configuration
# and include sub-projects here.
#
cmake_minimum_required (VERSION 3.19)

project("FlexIssue"
VERSION 1.0.0
LANGUAGES CXX
)

add_subdirectory("thirdparty")

add_executable(${PROJECT_NAME}   
   src/Main.cpp
) 

target_compile_features(${PROJECT_NAME} PRIVATE cxx_std_23)

target_link_libraries(${PROJECT_NAME}
    PUBLIC
    flecs::flecs
)
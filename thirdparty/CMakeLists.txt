cmake_minimum_required (VERSION 3.19)

include(FetchContent)

FetchContent_Declare(
    flecs
    GIT_REPOSITORY https://github.com/SanderMertens/flecs.git
    GIT_TAG "origin/master"
)
FetchContent_MakeAvailable(flecs)
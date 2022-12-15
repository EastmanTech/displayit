cmake_minimum_required(VERSION 3.20)

set(CMAKE_TOOLCHAIN_FILE "dependencies/vcpkg/scripts/buildsystems/vcpkg.cmake")

project("displayit"
    VERSION 0.0.1
    HOMEPAGE_URL "https://github.com/EastmanTech/displayit"
    LANGUAGES CXX
)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED TRUE)
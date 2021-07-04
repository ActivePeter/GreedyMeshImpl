cmake_minimum_required(VERSION 3.4)
project(MyApplication)

# options
option(Conan_SDL2 "use conan to load sdl2" ON)
if(Conan_SDL2)
    #conan
    include(${MyApplication_BINARY_DIR}/conanbuildinfo.cmake)
    conan_basic_setup()
endif()

set(CMAKE_MODULE_PATH "${PROJECT_SOURCE_DIR}/modules/" ${CMAKE_MODULE_PATH})

# Add Corrade as a subproject
add_subdirectory(third/corrade EXCLUDE_FROM_ALL)

# Add Magnum as a subproject, enable Sdl2Application
set(WITH_SDL2APPLICATION ON CACHE BOOL "" FORCE)
add_subdirectory(third/magnum EXCLUDE_FROM_ALL)

add_subdirectory(src)
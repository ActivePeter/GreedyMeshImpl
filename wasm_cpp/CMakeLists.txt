cmake_minimum_required(VERSION 3.4)

project(wasmTest)

set (CMAKE_CXX_STAND 11)

set(USE_FLAGS "-s WASM=1 -s USE_SDL=2 -o index.js")
set (CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} -std=c++11 ")


file(GLOB_RECURSE CORE_HDR src/*.h)
file(GLOB_RECURSE CORE_SRC src/*.cpp)


add_definitions(${USE_FLAGS})
#
# Trying usual cmake project compiler execution
#

add_executable(wasmTest ${CORE_SRC} ${CORE_HDR})
# set_target_properties(wasmTest 
#     PROPERTIES SUFFIX ".html"
#     LINK_FLAGS "-Os " ${USE_FLAGS})
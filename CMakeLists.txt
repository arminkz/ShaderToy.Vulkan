cmake_minimum_required(VERSION 3.10)

project(ShaderToyVulkan)

find_package(fmt CONFIG REQUIRED)

add_executable(ShaderToyVulkan main.cpp)

target_link_libraries(ShaderToyVulkan PRIVATE fmt::fmt)
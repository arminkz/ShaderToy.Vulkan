cmake_minimum_required(VERSION 3.10)

project(ShaderToyVulkan)

find_package(fmt CONFIG REQUIRED)
find_package(glfw3 CONFIG REQUIRED)
find_package(glm CONFIG REQUIRED)
find_package(Vulkan REQUIRED)

add_executable(ShaderToyVulkan main.cpp)

target_link_libraries(ShaderToyVulkan PRIVATE fmt::fmt)
target_link_libraries(ShaderToyVulkan PRIVATE glfw)
target_link_libraries(ShaderToyVulkan PRIVATE glm::glm)
target_link_libraries(ShaderToyVulkan PRIVATE Vulkan::Vulkan)

message(STATUS "I hate myself so I use cmake")


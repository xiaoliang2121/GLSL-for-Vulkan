cmake_minimum_required(VERSION 3.16)

project(vulkan_usage_example)

find_package(Vulkan REQUIRED)

add_executable(${PROJECT_NAME} main.c advanced.c)
target_link_libraries(${PROJECT_NAME} PRIVATE Vulkan::Vulkan)
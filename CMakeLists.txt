cmake_minimum_required(VERSION 4.1)
project(baglib)

set(CMAKE_CXX_STANDARD 20)
add_subdirectory(src)
set(GLFW_USE_WAYLAND ON)
target_link_libraries(baglib PRIVATE glfw)
target_link_libraries(baglib PRIVATE glm)
target_link_libraries(baglib PRIVATE vulkan)

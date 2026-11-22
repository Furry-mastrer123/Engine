cmake_minimum_required(VERSION 3.20)

project(Engine_HIY)

set(CMAKE_CXX_STANDARD 23)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

find_package(Vulkan REQUIRED)

set(VULKAN_SDK_PATH "C:\\VulkanSDK\\1.4.350.0")

include_directories("${VULKAN_SDK_PATH}/Include")
link_directories("${VULKAN_SDK_PATH}/Lib")


add_executable(Engine_HIY engine_start.cpp)
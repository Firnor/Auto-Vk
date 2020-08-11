cmake_minimum_required(VERSION 3.0)

project(auto-vk 
		LANGUAGES C CXX
		VERSION 1.0
		DESCRIPTION "Vulkan Convinience Layer")

add_library(${PROJECT_NAME} INTERFACE)
#target_sources(${PROJECT_NAME} INTERFACE src/avk.cpp src/sync.cpp)
target_include_directories(${PROJECT_NAME} INTERFACE include)
#find_library(VULKAN_LIB vulkan)
#target_link_libraries(${PROJECT_NAME} INTERFACE vulkan)
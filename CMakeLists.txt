cmake_minimum_required(VERSION 3.17.0)
project(vulkan_computing_example VERSION 0.1.0)

set(CMAKE_CXX_STANDARD 14)

# It is necessary to pass the DEBUG or RELEASE flag accordingly to Kompute
set(CMAKE_CXX_FLAGS_DEBUG "-DDEBUG=1")
set(CMAKE_CXX_FLAGS_RELEASE "-DRELEASE=1")

find_package(Vulkan REQUIRED)

add_executable(vulkan_computing
    main.cpp)

target_link_libraries(vulkan_computing
    Vulkan::Vulkan
)


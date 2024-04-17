cmake_minimum_required(VERSION 3.27)
project(dx11play)

set(CMAKE_CXX_STANDARD 17)

find_package(SDL2 REQUIRED)

add_executable(dx11play WIN32 main.cpp)

target_link_libraries(dx11play SDL2::SDL2)

target_compile_definitions(dx11play PUBLIC UNICODE)

target_include_directories(dx11play SYSTEM PRIVATE
        "C:\\Program Files (x86)\\Microsoft DirectX SDK (June 2010)\\Include"
)

target_link_directories(dx11play PRIVATE "C:\\Program Files (x86)\\Microsoft DirectX SDK (June 2010)\\Lib\\x64")
cmake_minimum_required(VERSION 3.10)

project(Arbore)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED True)

# Definitii pentru a evita conflictele intre Windows API si raylib
add_definitions(-DWIN32_LEAN_AND_MEAN)
add_definitions(-DRAUDIO_STANDALONE)

# Seteaza flag-ul care forteaza raylib sa redenumească functiile in conflict
add_definitions(-DPLATFORM_DESKTOP_SDL)

include_directories(sourceCode/include)

file(GLOB SOURCES "sourceCode/src/*.cpp")

# Configuram raylib inainte de a-l include ca subdirector
set(BUILD_EXAMPLES OFF CACHE BOOL "" FORCE)
set(BUILD_GAMES    OFF CACHE BOOL "" FORCE)
set(SUPPORT_SCREEN_CAPTURE OFF CACHE BOOL "" FORCE)

# Includem raylib ca un subdirector
add_subdirectory(buildTool/raylib)

# Cream executabilul 
add_executable(Arbore ${SOURCES})

# Link catre raylib
target_link_libraries(Arbore raylib)

# Adaugam definitia GRAPHICS_API_OPENGL_33 pentru a evita alte conflicte
target_compile_definitions(Arbore PRIVATE GRAPHICS_API_OPENGL_33)
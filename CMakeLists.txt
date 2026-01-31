cmake_minimum_required(VERSION 3.10)
project(my_cpp_project VERSION 0.1.0 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 17)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

if (MSVC)
  add_compile_options(/W4 /permissive-)
else()
  add_compile_options(-Wall -Wextra -Wpedantic -Wconversion)
endif()

include_directories(${PROJECT_SOURCE_DIR}/include)

add_executable(my_app
  src/main.cpp
  src/foo.cpp
)

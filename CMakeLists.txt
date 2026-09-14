cmake_minimum_required(VERSION 3.2.0)

find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})

target_sources(app PRIVATE src/main.c)

target_include_directories(app PRIVATE ../include)

add_subdirectory(lib)
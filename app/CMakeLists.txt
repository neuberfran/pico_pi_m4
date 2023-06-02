cmake_minimum_required(VERSION 3.20.0)

set(EXTRA_ZEPHYR_MODULES ${CMAKE_CURRENT_LIST_DIR})
find_package(Zephyr REQUIRED HINTS $ENV{ZEPHYR_BASE})
project(app)

target_sources(app PRIVATE src/main.c)

cmake_minimum_required(VERSION 3.13...3.27)

# initialize the SDK based on PICO_SDK_PATH
include(pico_sdk_import.cmake)

project(rp2350-dvitest)

pico_sdk_init()

add_subdirectory(dvitest)

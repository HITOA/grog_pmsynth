cmake_minimum_required(VERSION 3.16)
project(grog_pmsynth)

set(CMAKE_CXX_STANDARD 20)
set(CMAKE_CXX_STANDARD_REQUIRED ON)

if(NOT CMAKE_BUILD_TYPE)
  set(CMAKE_BUILD_TYPE Release)
endif()

add_subdirectory(grog_audio_plugin_client)

grog_add_plugin(grog_pmsynth
    FORMATS LV2 Standalone)
cmake_minimum_required(VERSION 3.28)
project(Aaron)

set(
SOURCE_FILES

    src/main.cpp
)

add_executable(Aaron ${SOURCE_FILES})
target_link_libraries(Aaron)

if(WIN32) 

    target_sources(Aaron PRIVATE Windows/app.rc)
endif()
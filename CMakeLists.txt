cmake_minimum_required (VERSION 2.8.11)
project (tweetnacl)
set (TWEETNACL_SOURCES tweetnacl.c)
add_library(tweetnacl_static STATIC ${TWEETNACL_SOURCES})
target_include_directories(tweetnacl_static
    PUBLIC ${CMAKE_CURRENT_SOURCE_DIR}
    )

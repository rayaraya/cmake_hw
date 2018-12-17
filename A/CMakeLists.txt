project(lib-proj)

add_library(Alib lib.c)
message(${CMAKE_CURRENT_SOURCE_DIR})

# Doesn't work: include_directories(PUBLIC ${PROJECT_SOURCE_DIR}/..), so use target_*
target_include_directories( Alib PUBLIC ${PROJECT_SOURCE_DIR}/..)


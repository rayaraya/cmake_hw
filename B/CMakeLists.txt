project(binary)


message(${CMAKE_CURRENT_SOURCE_DIR})
add_executable (main main.c)

target_link_libraries (main LINK_PUBLIC Alib)
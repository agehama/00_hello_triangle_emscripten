cmake_minimum_required(VERSION 2.8)

set(CMAKE_BUILD_TYPE Release)

add_executable(main main.c)
set_target_properties(main PROPERTIES LINK_FLAGS "${LINK_FLAGS} -s USE_GLFW=3 -s USE_REGAL=1 -s FULL_ES2=1")

set(CMAKE_EXECUTABLE_SUFFIX ".html")


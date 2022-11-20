# CMakeList.txt : CMake project for CSFML, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.20)

project ("CSFML" C)

# Add source to this project's executable.

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET CSFML PROPERTY CXX_STANDARD 20)
endif()

add_subdirectory(src)
add_subdirectory(external)
# TODO: Add tests and install targets if needed.

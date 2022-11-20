# CMakeList.txt : CMake project for CSFML, include source and define
# project specific logic here.
#
cmake_minimum_required (VERSION 3.20)

project ("CSFML" C)

# Add source to this project's executable.
add_executable (CSFML "src/CSFML.cpp" "CSFML.h")

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET CSFML PROPERTY CXX_STANDARD 20)
endif()


# TODO: Add tests and install targets if needed.

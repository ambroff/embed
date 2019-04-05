cmake_minimum_required(VERSION 3.9)

add_library(embed
  include/resource.hpp
  include/embed.hpp
  include/saver.hpp
  include/span.hpp
  src/main.cpp
  src/test
  src/test/test.cpp
  )

target_include_directories(embed PUBLIC
  $<BUILD_INTERFACE:${CMAKE_SOURCE_DIR}/include>
  )

cmake_minimum_required(VERSION 3.5)

set(n "http-parser")

project(${n})

add_library(${n}
  http_parser.c
)

target_include_directories(${n} PUBLIC .)

set_target_properties(${n} PROPERTIES PUBLIC_HEADER "http_parser.h")


cmake_minimum_required (VERSION 2.8.1)

PROJECT(hello)

file(GLOB hello_src hello.c)

add_executable(hello ${hello_src})
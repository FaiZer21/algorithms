cmake_minimum_required (VERSION 3.8)

project (algorithms-lib VERSION 0.1 LANGUAGES CXX)

set(CMAKE_CXX_STANDARD 11)
set(CMAKE_CXX_STANDARD_REQUIRED ON)
set(CMAKE_INCLUDE_CURRERNT_DIR ON)

set(SOURCES
	lib.h
	sum_of_unique.cpp
	sum_of_unique.hpp
	)

add_library(algorithms-lib ${SOURCES})

add_library(Algo::lib ALIAS algorithms-lib)

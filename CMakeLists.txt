
# Copyright (c) 2014-2016 Stefan.Eilemann@epfl.ch

cmake_minimum_required(VERSION 3.1 FATAL_ERROR)
project(HBPVIS VERSION 2016.04)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/CMake
  ${CMAKE_SOURCE_DIR}/CMake/common)

set(hbpvis_SKIP_FIND ON PARENT_SCOPE) # for superprojects

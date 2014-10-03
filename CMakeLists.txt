
# Copyright (c) 2014 Stefan.Eilemann@epfl.ch

cmake_minimum_required(VERSION 2.8 FATAL_ERROR)
project(HBPVis)

set(VERSION_MAJOR "2014")
set(VERSION_MINOR "6")
set(VERSION_PATCH "0")
set(GITTARGETS_RELEASE_BRANCH current)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR}/CMake
  ${PROJECT_SOURCE_DIR}/CMake/common)

include(GitExternal)
include(Common)

set(DOXYGIT_TOC_POST
  "<p>See also <a href='https://bluebrain.github.io'>bluebrain.github.io</a> <a href='https://eyescale.github.io'>eyescale.github.io</a></p>")
common_documentation()

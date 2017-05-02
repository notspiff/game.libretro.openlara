cmake_minimum_required(VERSION 3.1)
project(game.libretro.openlara)

list(APPEND CMAKE_MODULE_PATH ${PROJECT_SOURCE_DIR})

find_package(Kodi REQUIRED)
find_package(libretro-openlara REQUIRED)

set(OPENLARA_CUSTOM_BINARY ${OPENLARA_LIB}
    ${PROJECT_NAME}${CMAKE_SHARED_LIBRARY_SUFFIX})

build_addon(${PROJECT_NAME} OPENLARA "")

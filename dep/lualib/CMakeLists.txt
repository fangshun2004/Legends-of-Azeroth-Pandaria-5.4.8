# Copyright (C) 2008-2013 TrinityCore <http://www.trinitycore.org/>
#
# This file is free software; as a special exception the author gives
# unlimited permission to copy and/or distribute it, with or without
# modifications, as long as this notice is preserved.
#
# This program is distributed in the hope that it will be useful, but
# WITHOUT ANY WARRANTY, to the extent permitted by law; without even the
# implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
file(GLOB sources *.c)

set(lua_STAT_SRCS
  ${sources}
)

add_library(lua STATIC ${lua_STAT_SRCS})

target_include_directories(lua
  PUBLIC
    ${CMAKE_CURRENT_SOURCE_DIR}
)
###
#
#

include_directories(${CMAKE_CURRENT_SOURCE_DIR})
include_directories(${CMAKE_CURRENT_BINARY_DIR})

add_subdirectory(fixes)
add_subdirectory(sprokit)

if (KWIVER_ENABLE_TOOLS)
  add_subdirectory(tools)
endif ()

add_subdirectory(bindings)
add_subdirectory(processes)
add_subdirectory(schedulers)

# As part of installation we'll copy the examples
set(CMAKE_MODULE_PATH ${CMAKE_MODULE_PATH} "${CMAKE_CURRENT_SOURCE_DIR}/cmake")
include(X3D_ADD_EXAMPLE)
# Tests are in the folder tests
# This is only to have in the installation director the examples
set(examples_dir "${CMAKE_INSTALL_PREFIX}/examples")
install(DIRECTORY DESTINATION ${example_dir})

add_subdirectory(Cylinder-wake)
add_subdirectory(Periodic-hill)
add_subdirectory(Wind-Turbine)

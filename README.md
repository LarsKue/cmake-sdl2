FindSDL2.cmake
==============

FindSDL2 is a CMake module to locate SDL2 headers, libraries paths and additional linker flags. Following variables are provided:

  * SDL2_FOUND (True, if the system has SDL2.)
  * SDL2_INCLUDE_DIR (Path to the SDL2 include directory.)
  * SDL2_LIBRARIES (Paths to the SDL2 libraries.)
  * SDL2_LINK_FLAGS (Additional linker flags for SDL2.)
  * SDL2_SHARED_LIBRARY_PATH (Paths to the SDL2 shared library.)

### Example

    find_package(SDL2 REQUIRED)
    include_directories(${SDL2_INCLUDE_DIR})
    target_link_libraries(tgt ${SDL2_LIBRARIES})
    set_target_properties(tgt PROPERTIES LINK_FLAGS ${SDL2_LINK_FLAGS})


### Notes

On Microsoft Windows platform modules expect to have environment variable SDL2_ROOT_DIR defined.

cmake_minimum_required(VERSION 3.5)

project(LiverSegment)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://github.com/ljq2278/LiverSegment")
set(EXTENSION_CATEGORY "Examples")
set(EXTENSION_CONTRIBUTORS "JQ Lin (HuaQiao University)")
set(EXTENSION_DESCRIPTION "This is a module that can segment Liver from volume")
set(EXTENSION_ICONURL "https://raw.github.com/ljq2278/LiverSegment/master/LiverSegment.png")
set(EXTENSION_SCREENSHOTURLS "http://www.example.com/Slicer/Extensions/LiverSegment/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a space separated string, a list or 'NA' if any

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(LiverSegment)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})

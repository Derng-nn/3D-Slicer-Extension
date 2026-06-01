cmake_minimum_required(VERSION 3.20.6...3.22.6 FATAL_ERROR)

project(Tumor_Segmenatation)

#-----------------------------------------------------------------------------
# Extension meta-information
set(EXTENSION_HOMEPAGE "https://www.slicer.org/wiki/Documentation/Nightly/Extensions/Tumor_Segmenatation")
set(EXTENSION_CONTRIBUTORS "Noppanon Nobnop (Image Lab.)")
set(EXTENSION_DESCRIPTION "This is an example of a simple extension")
set(EXTENSION_ICONURL "https://www.example.com/Slicer/Extensions/Tumor_Segmenatation.png")
set(EXTENSION_SCREENSHOTURLS "https://www.example.com/Slicer/Extensions/Tumor_Segmenatation/Screenshots/1.png")
set(EXTENSION_DEPENDS "NA") # Specified as a list or "NA" if no dependencies

#-----------------------------------------------------------------------------
# Extension dependencies
find_package(Slicer REQUIRED)
include(${Slicer_USE_FILE})

#-----------------------------------------------------------------------------
# Extension modules
add_subdirectory(Tumor_Segmentation)
## NEXT_MODULE

#-----------------------------------------------------------------------------
include(${Slicer_EXTENSION_GENERATE_CONFIG})
include(${Slicer_EXTENSION_CPACK})

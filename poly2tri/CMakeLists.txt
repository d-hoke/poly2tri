include_directories(${CMAKE_CURRENT_SOURCE_DIR})

set(poly2tri_srcs
  common/shapes.cc
  sweep/advancing_front.cc
  sweep/cdt.cc
  sweep/sweep.cc
  sweep/sweep_context.cc
)

#if(MSVC)
#  add_definitions("-DP2T_DLL_EXPORTS")
#endif(MSVC)

  add_library(poly2tri-static STATIC ${poly2tri_srcs})

# Local Variables:
# tab-width: 8
# mode: cmake
# indent-tabs-mode: t
# End:
# ex: shiftwidth=2 tabstop=8


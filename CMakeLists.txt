cmake_minimum_required (VERSION 2.6)
project (MT3D)
enable_language( Fortran )
set( Toolchain gFortran )

file(GLOB mt3d_SRC "*.f" "mt_module.f90")

add_executable(mt3d ${mt3d_SRC})

SET_TARGET_PROPERTIES(mt3d PROPERTIES LINKER_LANGUAGE Fortran)

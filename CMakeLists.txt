project( LAPACKE_examples )
cmake_minimum_required( VERSION 2.6 )

include_directories( ${CMAKE_SOURCE_DIR}/include )
link_directories( ${CMAKE_SOURCE_DIR}/lib )
set( libs   "liblapacke.lib;liblapack.lib; libblas.lib;"
            "kernel32.lib;user32.lib;gdi32.lib;winspool.lib;"
            "comdlg32.lib;advapi32.lib;shell32.lib;ole32.lib;"
            "oleaut32.lib;uuid.lib;odbc32.lib;odbccp32.lib" )
add_subdirectory( examples )

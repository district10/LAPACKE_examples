set( examples
    example_DGESV_rowmajor
    example_ZGESV_rowmajor
)

foreach( example ${examples} )
    add_executable( ${example} ${example}.c )
    set_source_files_properties( ${example}.c PROPERTIES LANGUAGE C )
    target_link_libraries( ${example} libs )
endforeach( example )

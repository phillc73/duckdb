add_library_unity(duckdb_func_string
                  OBJECT
                  reverse.cpp
                  caseconvert.cpp
                  concat.cpp
                  length.cpp
                  like.cpp
                  printf.cpp
                  regexp.cpp
                  substring.cpp)
set(ALL_OBJECT_FILES
    ${ALL_OBJECT_FILES} $<TARGET_OBJECTS:duckdb_func_string>
    PARENT_SCOPE)

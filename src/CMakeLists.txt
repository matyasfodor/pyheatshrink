set(HEADER_FILES dynamic_arrays.h)
set(SOURCE_FILES heatshrink.c dynamic_arrays.c)

set(ALL_FILES ${HEADER_FILES} ${SOURCE_FILES})

add_library(pyheatshrink ${ALL_FILES})

# Install includes
install(FILES ${HEADER_FILES} DESTINATION include/pyheatshrink)

# Install library files
# install(TARGET pyheatshrink
#   LIBRARY DESTINATION lib
#   ARCHIVE DESTINATION lib)

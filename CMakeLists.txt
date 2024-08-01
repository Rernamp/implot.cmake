

set(ImplotFolder ${CMAKE_CURRENT_SOURCE_DIR}/implot)

add_library(Implot INTERFACE)
target_include_directories(Implot INTERFACE
    ${ImplotFolder}
)

target_sources(Implot INTERFACE
    ${ImplotFolder}/implot.cpp
    ${ImplotFolder}/implot.h
    ${ImplotFolder}/implot_internal.h
    ${ImplotFolder}/implot_items.cpp
    ${ImplotFolder}/implot_demo.cpp
)
add_executable(dvitest
        dvitest.c
        )

target_include_directories(dvitest PRIVATE
        ${CMAKE_CURRENT_LIST_DIR}/images
        )

# pull in common dependencies
target_link_libraries(dvitest
        pico_stdlib
        pico_multicore
        hardware_dma
        pico_sync
        )

# create map/bin/hex/uf2 file etc.
pico_add_extra_outputs(dvitest)

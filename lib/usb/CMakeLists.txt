
target_sources(dev_hid_composite PUBLIC
${CMAKE_CURRENT_LIST_DIR}/main.c
${CMAKE_CURRENT_LIST_DIR}/usb_descriptors.c
)
pico_add_extra_outputs(dev_hid_composite)

add_executable(${PROJECT_NAME}
        mouse.h
        keyboard.h
        usb.cpp
        )
add_subdirectory(tinyusb)


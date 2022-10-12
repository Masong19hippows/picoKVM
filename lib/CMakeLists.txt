add_subdirectory(usb)
add_subdirectory(web)


# In addition to pico_stdlib required for common PicoSDK functionality, add dependency on tinyusb_device
# for TinyUSB device support and tinyusb_board for the additional board support library used by the example
target_link_libraries(dev_hid_composite PUBLIC pico_stdlib tinyusb_device tinyusb_board)
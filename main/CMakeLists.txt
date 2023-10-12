set(srcs "esp_hid_device_main.cpp"
         "esp_hid_gap.c"
         "utility/Keyboard.cpp"
         "esp_hid_gap.c"
         )
set(include_dirs "." "utility")

idf_component_register(SRCS "${srcs}"
                       INCLUDE_DIRS "${include_dirs}"
                       REQUIRES esp_hid M5GFX M5Unified)

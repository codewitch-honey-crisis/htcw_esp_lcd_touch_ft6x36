cmake_minimum_required(VERSION 3.24)

# ESP-IDF component
idf_component_register(
    SRCS "./src/source/esp_lcd_touch_ft6x36.c"
    INCLUDE_DIRS "." "./src"
    REQUIRES driver freertos esp_lcd        # add this (or PRIV_REQUIRES — see below)
)

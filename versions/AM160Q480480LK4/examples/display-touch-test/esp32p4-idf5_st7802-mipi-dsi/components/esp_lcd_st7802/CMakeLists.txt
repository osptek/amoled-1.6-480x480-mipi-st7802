idf_component_register(SRCS "esp_lcd_st7802_spi.c" "esp_lcd_st7802_mipi.c" "esp_lcd_st7802.c"
                       INCLUDE_DIRS "include"
                       PRIV_INCLUDE_DIRS "priv_include"
                       REQUIRES "esp_lcd" "driver")



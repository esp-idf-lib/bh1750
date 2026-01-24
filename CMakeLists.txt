list(APPEND CMAKE_MODULE_PATH ${CMAKE_CURRENT_LIST_DIR}/eil-cmake-utils/cmake)

idf_component_register(
    SRCS bh1750.c
    INCLUDE_DIRS .
    REQUIRES i2cdev log esp_idf_lib_helpers
)

include(eil_ci)

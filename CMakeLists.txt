add_library(fingerprint-lib STATIC
    Adafruit_Fingerprint.cpp
)

target_include_directories(fingerprint-lib
    INTERFACE
        .
)

target_link_libraries(fingerprint-lib 
    PUBLIC 
    mbed-core-flags
) # This is needed so that the library can access Mbed includes


VScode platformio arduino ESP-S3


.pio/libdeps/esp32dev/ESP32Encoder/src/ESP32Encoder.cpp: In function 'void esp32encoder_pcnt_intr_handler(void*)':
.pio/libdeps/esp32dev/ESP32Encoder/src/ESP32Encoder.cpp:51:24: error: 'volatile union pcnt_un_status_reg_t' has no member named 'h_lim_lat'
  #define COUNTER_H_LIM h_lim_lat
                        ^~~~~~~~~
.pio/libdeps/esp32dev/ESP32Encoder/src/ESP32Encoder.cpp:62:27: note: in expansion of macro 'COUNTER_H_LIM'
    if(PCNT.status_unit[i].COUNTER_H_LIM){
                           ^~~~~~~~~~~~~
.pio/libdeps/esp32dev/ESP32Encoder/src/ESP32Encoder.cpp:52:24: error: 'volatile union pcnt_un_status_reg_t' has no member named 'l_lim_lat'
  #define COUNTER_L_LIM l_lim_lat
                        ^~~~~~~~~
.pio/libdeps/esp32dev/ESP32Encoder/src/ESP32Encoder.cpp:65:34: note: in expansion of macro 'COUNTER_L_LIM'
    } else if(PCNT.status_unit[i].COUNTER_L_LIM){
                                  ^~~~~~~~~~~~~
.pio/libdeps/esp32dev/ESP32Encoder/src/ESP32Encoder.cpp:68:65: error: 'volatile union pcnt_un_status_reg_t' has no member named 'thres0_lat'
    } else if(esp32enc->always_interrupt && (PCNT.status_unit[i].thres0_lat || PCNT.status_unit[i].thres1_lat)) {
                                                                 ^~~~~~~~~~
.pio/libdeps/esp32dev/ESP32Encoder/src/ESP32Encoder.cpp:68:99: error: 'volatile union pcnt_un_status_reg_t' has no member named 'thres1_lat'
    } else if(esp32enc->always_interrupt && (PCNT.status_unit[i].thres0_lat || PCNT.status_unit[i].thres1_lat)) {
                                                                                                   ^~~~~~~~~~
*** [.pio\build\esp32dev\lib639\ESP32Encoder\ESP32Encoder.cpp.o] Error 1

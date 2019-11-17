# esphome-nodes

The nodes are built to be used together with [ESPHome](https://esphome.io) and [Home Assistant](home-assistant.io).

## display_node

The `display_node.yaml` is using the [Waveshare E-Paper ESP32 Driver Board](https://www.waveshare.com/wiki/E-Paper_ESP32_Driver_Board) 
toghether with a [4.2inch e-Paper Module](https://www.waveshare.com/wiki/4.2inch_e-Paper_Module) directly connected. Note the following connection used in ESPHome:

```yaml
spi:
  clk_pin: 13
  mosi_pin: 14

display:
  - platform: waveshare_epaper
    id: epaper
    cs_pin: 15
    busy_pin: 25
    reset_pin: 26
    dc_pin: 27
    ```
]

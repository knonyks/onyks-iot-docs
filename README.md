# ONYKS IoT - Dokumentacja

## 14.11.2024

### Z czego korzystamy

- moduł [ESP32-WROOM-32D](https://www.espressif.com/sites/default/files/documentation/esp32-wroom-32d_esp32-wroom-32u_datasheet_en.pdf)
- program [KiCAD](https://www.kicad.org/) w wersji 8
- GitHub do przechowywania projektów

### Co zrobić do następnego spotkania

- zastanowić się jak ma działać urządzenie
- znaleźć główne peryferia spełniajace założenia projektu
- zaplanowanie maksymalnego poboru prądu przez dobrane peryferia
  - nie projektujemy jeszcze układu zasilania
- opcjonalnie: mały schemat w [drawio](https://app.diagrams.net/)
- zapoznać się z przykładowym devbardem

### Gdzie czytać

- oficjalny [devboard](https://docs.espressif.com/projects/esp-dev-kits/en/latest/esp32/esp32-devkitc/user_guide.html) - warto zapoznać się
  - na dole jest dokumentacja: specyfikacja techniczna, schematy, płytka PCB
- wprowadzenie do [KiCADa](https://docs.kicad.org/8.0/en/getting_started_in_kicad/getting_started_in_kicad.html)
- na przyszłość, można czytać w wolnej chwili [wprowadzenie do ESP32](https://docs.espressif.com/projects/esp-idf/en/v5.3.1/esp32/get-started/index.html)

### Podstawowe założenia

- zasilanie 3,3 V
- komunikacja Bluetooth (na tym etapie projektu to tylko ciekawostka)
- nie będzie programatora na płytce (programatory będą osobno)
- interfejsy UART i JTAG do programowania i debuggowania
- przycisk "reset"

### Components

- LDO: SOT-23-5 (DYD) [TLV75733PDBVR](https://www.ti.com/lit/ds/symlink/tlv757p.pdf?ts=1733149199380&ref_url=https%253A%252F%252Fwww.ti.com%252Fproduct%252FTLV757P%252Fpart-details%252FTLV75710PDBVR)
- NPN: SOT-23-3 [SS8050](https://www.micros.com.pl/mediaserver/TSS8050_BORN_0001.pdf)
- LED: 5050 [WS2812B](https://cdn-shop.adafruit.com/datasheets/WS2812B.pdf)
- Buttons: [6x3.5mm](https://pl.aliexpress.com/item/4000546183248.html?spm=a2g0o.order_list.order_list_main.169.6deb1c24ZkOZZl&gatewayAdapt=glo2pol) np. `Button_Switch_SMD:SW_Tactile_SPST_NO_Straight_CK_PTS636Sx25SMTRLFS`

### Connectors

- UART for programming
  1. VCC (3.3V)
  2. GND
  3. TXD (UART Transmit)
  4. RXD (UART Receive)
  5. EN (Enable/Reset)
  6. GPIO0 (Boot mode selection)

- JTAG for debugging (TMS, TCK, TDI, TDO, GND)

- UART for communication

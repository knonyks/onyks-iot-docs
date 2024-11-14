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
- interfejsy JTAG i USB do programowania i debuggowania
- przycisk "reset"

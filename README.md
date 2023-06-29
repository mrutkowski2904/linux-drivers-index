# Linux drivers index
This repository contains an overview of the Linux drivers that I wrote:

* **Realtek RTL8169 Ethernet Driver** <br>
  Driver for RTL8169 PCI Ethernet Card. Supports Gigabit Ethernet. <br>
  DMA is used for data transfers. Uses MMIO.  <br>
  Link: [https://github.com/mrutkowski2904/rtl8169-linux-network-driver](https://github.com/mrutkowski2904/rtl8169-linux-network-driver)
  
* **Wi-Fi network driver that uses ESP32 C3 module as a network adapter** <br>
  Uses `cfg80211` subsystem for Wi-Fi. Supports sending and receiving network data. <br>
  The following Wi-Fi STA operations are supported: scanning/connecting/disconnecting <br>
  Link: [https://github.com/mrutkowski2904/esp-linux-network-driver](https://github.com/mrutkowski2904/esp-linux-network-driver)

* **Block driver for W25Q128JV flash memory** <br>
  Uses `blk-mq` framework. The memory can be mounted, unmounted and formatted like a typical drive <br>
  Link: [https://github.com/mrutkowski2904/w25q128jv-linux-block-driver](https://github.com/mrutkowski2904/w25q128jv-linux-block-driver)

* **Framebuffer display driver for ILI9341 display** <br>
  DMA is used for data transfers. Supports 18-bit color depth (max supported value by ILI9341) <br>
  Link: [https://github.com/mrutkowski2904/ili9341-linux-display-driver](https://github.com/mrutkowski2904/ili9341-linux-display-driver)

* **Framebuffer display driver for SSD1306 display** <br>
  Driver for cheap SSD1306 monochrome display <br>
  Link: [https://github.com/mrutkowski2904/ssd1306-linux-display-driver](https://github.com/mrutkowski2904/ssd1306-linux-display-driver)

* **GPIO driver for MCP23008 GPIO expander** <br>
  Supports interrupts on expander pins. The driver uses `regmap` API. <br>
  Link: [https://github.com/mrutkowski2904/mcp23008-linux-gpio-driver](https://github.com/mrutkowski2904/mcp23008-linux-gpio-driver)

* **Driver for LPS25HB barometer** <br>
  Pressure can be read in blocking or non blocking mode. `sysfs` attribute is used for driver configuration. <br>
  Link: [https://github.com/mrutkowski2904/lps25hb-barometer-linux-driver](https://github.com/mrutkowski2904/lps25hb-barometer-linux-driver)

Few of these drivers were originally developed in the repository of my [weather station](https://github.com/mrutkowski2904/weather-station-buildroot) project and were later moved to separate repositories. To see their commit history, check my weather station project.

# Wi-Fi SoftAP Example

This example shows how to use the Wi-Fi SoftAP functionality of the Wi-Fi driver of ESP for serving as an Access Point.

## How to use example

### Configure the project

Open the project configuration menu (`idf.py menuconfig`). 

In the `Example Configuration` menu:

* Set the Wi-Fi configuration.
    * Set `WiFi SSID`.
    * Set `WiFi Password`.

Optional: If you need, change the other options according to your requirements.

### Build and Flash

Build the project and flash it to the board, then run the monitor tool to view the serial output:

Run `idf.py -p PORT flash monitor` to build, flash and monitor the project.

(To exit the serial monitor, type ``Ctrl-]``.)

See the Getting Started Guide for all the steps to configure and use the ESP-IDF to build projects.

* [ESP-IDF Getting Started Guide on ESP32](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/get-started/index.html)

## Example Output

There is the console output for this example:

```
I (657) phy_init: phy_version 4670,719f9f6,Feb 18 2021,17:07:07
I (767) wifi:mode : softAP (24:0a:c4:1c:7e:f1)
I (777) Web Server: wifi_init_softap finished. SSID:NIRAV password:12345678 channel:1
I (187987) wifi:new:<1,1>, old:<1,1>, ap:<1,1>, sta:<255,255>, prof:1
I (187987) wifi:station: 3a:61:1e:d1:2a:4a join, AID=1, bgn, 40U
I (188077) Web Server: station 3a:61:1e:d1:2a:4a join, AID=1
I (188187) wifi:<ba-add>idx:2 (ifx:1, 3a:61:1e:d1:2a:4a), tid:0, ssn:0, winSize:64
I (188277) esp_netif_lwip: DHCP server assigned IP to a station, IP is: 192.168.4.2
I (256667) Web Server: LED TURNED ON
I (256667) Web Server: response sent successfully
I (260197) Web Server: LED TURNED OFF
I (260207) Web Server: response sent successfully
```


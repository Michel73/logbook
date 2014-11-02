# HowTo Setup RaspberryPi WiFi and Webcam to build a Watchdog for my heat pump

## Parts

* RaspberryPi
* Edimax WiFi
* Webcam 
* LED light

## Setup WiFi

Followed instructions in [How-To: Add WiFi to the Raspberry Pi](http://raspberrypihq.com/how-to-add-wifi-to-the-raspberry-pi/)

```bash
dmesg | more
sudo vi /etc/network/interfaces
```

contents

```
auto lo
iface lo inet loopback
iface eth0 inet dhcp

allow-hotplug wlan0
auto wlan0

iface wlan0 inet dhcp
   wpa-ssid "Your Network SSID"
   wpa-psk "Your Password"
```

Edit you SSID and PSK and save the file.

```bash
sudo service networking reload
ifconfig
```

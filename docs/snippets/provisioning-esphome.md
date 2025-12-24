<!-- Add product specific variables once component system is ready -->
<!-- Read more: https://zensical.org/about/roadmap/#component-system -->
=== ":fontawesome-solid-wifi: WiFi Provisioning"
    1. Connect the device to a power supply.
    1. On your phone or computer, connect to the temporary WiFi network (e.g. ==bed-presence-xxxxxx==).
    1. If your device prompts you to "stay connected", tap ==Yes==.
    1. Open a web browser and navigate to ==http://192.168.4.1==.
    1. Select the WiFi network you want the device to join, enter its password, and tap ==Save==.
        - The ESP will now try to connect to the network...but it will not provide confirmation.
        - Continue to [Platform Setup](platform-setup.md)

=== ":fontawesome-brands-bluetooth: BT Provisioning"
    If you are using Home Assistant and have a Bluetooth Proxy, simply connect power to the device and continue to [Platform Setup](platform-setup).

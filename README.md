phone-bridge
============

Howto bridge (via a usb-tethered phone) to the internet, on a Raspberry-Pi running Arch Linux

On a clean installation of Arch Linux, place the three files (phonebridge.sh, tether and usbbridge)
into /usr/local/bin and then place phonebridge.service into /etc/systemd/system and then install
it by doing

$ systemctl enable phonebridge

**1.)** Reboot the Raspberry Pi

**2.)** Plug your ethernet device (probably a router) into the Pi's LAN port

**3.)** Tether the phone to the Raspberry Pi over usb

**4.)** After the pi settles down a bit, and the phone notices that it's tethered, click the phone setting that enables tethering

**5.)** The Pi's leds will flicker and after a while, the router will light up its "connected to the internet" led - yay!


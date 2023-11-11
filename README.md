# Enable IPV6 on Huawei Moded Modem(V7R11)

Requirements:
1. Putty
2. XAMPP

Steps:
1. Download fixipv6 to the pc.
2. Connect pc to modem using LAN cable.
3. Open XAMPP and enable apache.
4. Login to the modem as Telnet(Port 23) by Putty as root@192.168.8.1
5. Type cd /tmp/ then press enter.
6. Type chmod 755 fixipv6 then press enter.
7. Type ./fixipv6 then press enter.
8. After the script was finished, type reboot then press enter. The modem will be reboot.

This process will reset the modem to factory default. The administration login will change as admin:admin. WiFi SSID and Password need to be set after the process.

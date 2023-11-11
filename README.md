# Enable IPV6 on Huawei Moded Modem v11

Requirements:
1. Putty
2. WinSCP

Steps:
1. Download fixipv6 to the pc.
2. Transfer fixipv6 to the modem thru WinSCP at directory /tmp/
3. Login to the modem as Telnet(Port 23) by Putty as root@192.168.8.1
4. Type cd /tmp/ then press enter.
5. Type chmod 755 fixipv6 then press enter.
6. Type ./fixipv6 then press enter.
7. After the script was finished, type reboot then press enter. The modem will be reboot.

This process will reset the modem to factory default. The administration login will change as admin:admin. WiFi SSID and Password need to be setting after process.

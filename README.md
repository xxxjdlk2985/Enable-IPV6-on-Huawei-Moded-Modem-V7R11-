# Enabling IPV6 on Huawei Moded Modem(V7R11)

Requirements:
1. Putty
2. XAMPP
3. Enabled ADB Telnet on the modem

Steps:
1. Download fixipv6 to the pc.
2. Connect pc to modem using LAN cable.
3. Open XAMPP and start apache.
4. Copy fixipv6 to XAMPP directory : C:\xampp\htdocs\dashboard
5. Go to browser and surf http://localhost/ to confirm that apache server is working.
6. Open CMD, type ipconfig then press enter to get ipv4 address for pc.
7. Login to the modem as Telnet(Port 23) by Putty as root@192.168.8.1
8. Type cd /tmp/ then press enter.
9. Type busybox-1.31.1 wget http://ip.pc/dashboard/fixipv6. Replace ip.pc with ipv4 address for pc from CMD. then press enter.
10. Type chmod 755 fixipv6 then press enter.
11. Type ./fixipv6 then press enter.
12. After the script was finished, type reboot then press enter. The modem will be reboot.

This process will reset the modem to factory default. The administration login will change as admin:admin. WiFi SSID and Password need to be set after the process.

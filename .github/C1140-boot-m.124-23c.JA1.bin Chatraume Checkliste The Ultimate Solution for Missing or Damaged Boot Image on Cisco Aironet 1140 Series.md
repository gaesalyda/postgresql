
 
# How to Load a Boot Image to Cisco Aironet 1140 Series After Missing C1140-boot-m.124-23c.JA1.bin File
 
If you have a Cisco Aironet 1140 series access point that is blinking with a red light and gives a message "no boot image to load", you may have accidentally deleted or corrupted the C1140-boot-m.124-23c.JA1.bin file from its flash memory. This file is the boot loader image that allows the access point to load the IOS image and operate normally. Without it, the access point cannot boot up and function.
 
Fortunately, there is a way to recover the access point by loading a new boot image file from a TFTP server. This article will guide you through the steps to do so, as well as provide a checklist of things to prepare before you start.
 
**Download File › [https://t.co/JYU7a0Lm7M](https://t.co/JYU7a0Lm7M)**


 
## Chatraume Checkliste
 
- A TFTP server that is reachable from the access point's Ethernet interface. You can use any TFTP server software that you prefer, such as TFTPD32, SolarWinds TFTP Server, or Cisco TFTP Server.
- A C1140-boot-m.124-23c.JA1.bin file that matches the model and IOS version of your access point. You can download it from Cisco's website or copy it from another working access point of the same model and IOS version.
- A console cable that connects your PC to the access point's console port. You will need a terminal emulation software such as PuTTY, HyperTerminal, or SecureCRT to communicate with the access point.
- A power source for the access point. You can use a power injector, a power adapter, or a PoE switch to provide power to the access point.

## Steps to Load a Boot Image

1. Connect your PC to the access point's console port using the console cable and launch your terminal emulation software. Set the baud rate to 9600, data bits to 8, parity to none, stop bits to 1, and flow control to none.
2. Connect your PC to the same network as the TFTP server using an Ethernet cable. Make sure you have an IP address that is in the same subnet as the TFTP server.
3. Connect the access point's Ethernet port to the same network as the TFTP server using another Ethernet cable.
4. Power on the access point and wait for it to boot up. You should see some messages on your terminal screen indicating that the access point is trying to load the boot image file from flash memory.
5. When you see the message "no boot image to load", press Esc on your keyboard to interrupt the boot process. You should see a prompt that says "ap:".
6. Type "set" and press Enter to see the current environment variables of the access point. Take note of the values of BOOTLDR, DEFAULT\_ROUTER, IP\_ADDR, NETMASK, and TFTP\_SERVER.
7. Type "set BOOTLDR flash:c1140-boot-m.124-23c.JA1.bin" and press Enter to set the boot loader image file name.
8. Type "set DEFAULT\_ROUTER <ip address="" of="" your="" default="" gateway="">" and press Enter to set the default gateway for the access point.</ip>
9. Type "set IP\_ADDR <ip address="" for="" your="" access="" point="">" and press Enter to set an IP address for your access point that is in the same subnet as the TFTP server.</ip>
10. Type "set NETMASK <subnet mask="" for="" your="" network="">" and press Enter to set the subnet mask for your network.</subnet>
11. Type "set TFTP\_SERVER <ip address="" of="" your="" tftp="" server="">" and press Enter to set the IP address of your TFTP server.</ip>
12. Type "tftp\_init" and press Enter to initialize the TFTP client on the access point.
13. Type "ether\_init" and press Enter to initialize the Ethernet interface on the access point.
14. Type "tar -xtract tftp://<ip address="" of="" your="" tftp="" server="">/c1140-boot-m.124-23c
<p>C1140-boot-m.124-23c.JA1.bin chatraume checkliste download, 
How to use C1140-boot-m.124-23c.JA1.bin chatraume checkliste, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste tutorial, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste features, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste review, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste alternative, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste update, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste error, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste manual, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste guide, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste installation, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste configuration, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste troubleshooting, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste support, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste forum, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste tips, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste best practices, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste comparison, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste benefits, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste advantages, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste disadvantages, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste limitations, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste requirements, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste compatibility, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste price, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste free trial, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste demo, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste license, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste warranty, 
C1140-boot-m.124-23c.JA1.bin chatraume checkliste refund policy</p> 8cf37b1e13


</ip>
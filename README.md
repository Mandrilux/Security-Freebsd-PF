# Security-Freebsd-PF
This firewall allow protects different attacks and allow only legitimate packets to enter in you server

you can change the port , and ip , it's paquet filter firewall
If you block IP or range IP , you can put IP in /banip.txt

exemple if you ban IP 192.1.2.1 , put in /banip.txt
192.1.2.1

exemple if you ban network 192.1.2.0/24 , put in /banip.txt
192.1.2.0/24

execute this commande for start the kernel module:
kldload pf

you need to add this line in /etc/rc.conf for start PF automatically
pf_enable="YES"
pf_rules="/etc/pf.conf"


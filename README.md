# Firewalls
A firewall is basically a network security system, available as either hardware or software, that acts as a barrier between a trusted internal network and untrusted external networks, like the internet, to prevent unauthorized access. It works by monitoring and filtering incoming and outgoing network traffic based on predefined security rules, deciding to allow or block specific data based on criteria like IP addresses and protocols to protect against threats and malicious actors
---

**Linux Firewall (using ufw )**
UFW, which stands for Uncomplicated Firewall, is a user-friendly command-line tool for managing the Linux iptables firewall, simplifying network traffic control on Linux systems, especially Ubuntu. It provides a simpler interface for configuring firewall rules to allow or block access to ports, IP addresses, and services.

**Installation & Steps**
1. sudo apt install uwf -y
2. sudo ufw enable
3. sudo ufw allow ssh ( filtering based on service)
4. sudo ufw allow 22  ( filtering based on port)
5. sudo ufw deny 80   ( Blocking a specific port)
6. sudo ufw allow from 192.168.1.50 ( filtering from a specific source)

**Testing**
Try connecting to the machine with SSH when allowed → it should work.<br>
Block SSH and try again → it should fail.<br>
Use curl http://<ip> to test blocked vs allowed HTTP.<br>







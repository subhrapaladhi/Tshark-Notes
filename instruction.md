## View active network interface
### ifconfig
The “ifconfig” command with no arguments will display all the active interfaces details. The ifconfig command also used to check the assigned IP address of an server.

## View all network interface
### ifconfig -a
The ifconfig command with -a argument will display information of all active or inactive network interfaces on server. 

## View a specific network interface
### ifconfig <interface name>
eg: ```ifconfig wlp2s0```

## Get your public IP
### wget -qO- ifconfig.me

## Monitor packets on a network interface
### sudo tshark -i <interface name>
eg: ```sudo tshark -i wlp2s0```

## Install bind-utils
```sudo apt install bind9-utils```

## See your nameserver
```cat /etc/resolv.conf```

## nslookup
### nslookup <domin>
eg: ```nslookup textsummarizer.subhrapaladhi.com```

## Question: 
Q. why is IP 224.0.0.251 trying to connect to me when I log into my gmail?
A. 224.anything and 192.anything are devices or apps on your local network (home/school/work). 192.anything especially is another device on that same network. The other ones included a 192.* type, which I've already described.
The FF02::FB is probably a portion of an IPv6 ip address. 224.* is a multicast "domain", wherein various apps will use it to connect to other apps etc.


## TCP Handshake
![TCP Handshake example]("./tcpHandshake.png")
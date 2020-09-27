- IP Addreses
- Mac Addresses
- TCP, UDP and the Three - Way Handshake
- Common Ports and Protocols
- The OSI Model
- Subnetting

\\\\\\\ IP addresses /////////

Why we use ip address. We use kali linux terminal and we are writing -ifconfig 
if u are in windows u can write ipconfig.
inet is our ip addres.
inet is ipv4.
inet6 is ipv6.

inet is a decimal notation and ipv6 (inet6) is in a hexadecimal notation.
inet(ipv4) is how we commubnicate. 
we communicate over layer 3.
ip adrdresses are layer 3 protocols layer 3 is a router.

\\\\\\\ MAC addresses /////////

our pyhsical address.

we learn mac address is which device with mac adress lookup.
00:2a:2A go to mac adress lookup and after than search learn which device is make connect device.
ether is our mac adress
put those into the google machine and see if you can identify what that device is.
Mac addreses layer two.
related to switching.

\\\\\\\  TCP, UDP and the Three - Way Handshake addresses /////////
layer four which is the transport layer of the osı model 
TCP : Transmission control protocol.
connection oriented protocol like web site 
http or https file transfer protocol
tcp works on what is called a three way handskae
syn packet > syn ack packet > ack packet
syn packet say "hello"
syn ack going to be the response it's going to say hey syn i acknowledge you hello back


UDP : user datagram protocol
connection less protocol
streaming service
that's connection lists or dns connections or voice over ip is connection lists.

Http that's over port 80
Https that's over port 443


you want to connect to port 443 on a web site you're going to send out a send packet
to that web site you²re going to say hey i want to connect to you on port 443 and if 
for 4 or 3 is open and available for connection they're going to say hey you can go
ahead and connect to me.

\\\\\\\  Common Ports and Protocols/////////

TCP                                                                               UDP
-FTP (21)                                                                       DNS (53)
-SSH (22)                                                                      DHCP(67,68)
-Telnet (23)                                                                    TFTP (69)
-SMTP (25)                                                                    SNMP(161)
-DNS (53)
-HTTP (80) / HTTPS (443)
-POP3 (110)
-SMB (139+445)
-IMAP (143)


FTP : File transfer protocol 
You're going to see this in some assessments you're going to see this a lot when we do something called capture the flag.
all that means is we can log into the server.

SSH and TELNET:
Kind of play hand in hand telnet is the ability to log into a machine remotely.
SSH does same things.
The only difference SSH is the encrypted version of that.

SMTP, POP3 and IMAP:
all relate to mail.

DNS:
DNS is a way to resolve IP addresses to names.

HTTP and HTTPS:
That is a web site just what you saw there
HTTP is not encrypted and not secure protocol.

SMB:
There relate to file share as you might also hear this called samba.

DHCP : 
Associates you witch an IP address kind of at random.
You could have the opposite of that is what is a static ip address.
So with DHCP you plug into your network say your home network and
the internet just fires up.

TFTP: 
like ftp but easy funciton than ftp protocol. File transfer protocol

SNMP : 
The simple network management protocol.

\\\\\\\ The OSI Model/////////

1 Physical - data cables, cat6
2 Data - Switching, Mac addresses
3 Network - IP addreses, routing
4 Transport - TCP/UDP
5 Session - sesssion management
6 Presentation - WMV, JPEG,MOVE
7 Application - HTTP,SMTP

(please do not throw sausage pizza away)

About too with the osi model is when we receive data we receive data down the physical layer all the way down the application when we transmit data.
It goes out the application layer down to the physical when we're troubleshooting this.
It is always best to start with a physical and go down to he apllication level.


\\\\\\\Subnetting/////////

netmask 255.255.255.0 all part consist of 8 bits

So 255: 1 1 1 1 1 1 1 1

2^0 *1 =  1
2^1 * 1=  2
2^2 * 1 =  4
2^3 * 1 =  8 
2^4 * 1= 16
2^5 * 1 = 32
2^6 * 1 = 64
2^7 * 1 = 128

all parts sum are 255 

Hosts :   128  64  32  16     8     4    2    1
Subnet : 128 192 224 240 248 252 254 255 

we add subnet numbers to cross the numbers   

8 bits : 255.0.0.0
16 bits : 255.255.0.0
24 bits : 255.255.255.0
32 bits : 255.255.255.255

Hosts double each increment of a CIDR
Always substract 2 from host total:
Network ID - First Address
Broadcast - Last Address



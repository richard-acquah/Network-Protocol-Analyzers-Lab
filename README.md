# Network Protocol Analysis With Wireshark

## Objectives
This lab seeks to demonstrate how Wireshark is installed on a Windows 10 virtual machine and how it is used to capture network traffic. The primary focus of this lab was to capture traffic traversing the Windows 10 virtual machine interface card and review the captured traffic.

## Skills Learned
+ Enhanced knowledge of network protocols.
+ Packet analysis.

## Resources / Tools / Utilities
+ Windows 10 virtual machine.
+ Wireshark.
+ Internet access.

## Steps - Section A
To install Wireshark, open the browser, enter the URL www.wireshark.org and click Get Started.

<img width="657" alt="wireshark downl1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/4f53e168-f8b7-4773-952e-309534b59df8">

##

Click the Windows x64 installer to download, click the open file after downloading to launch the setup wizard and click Next.

<img width="650" alt="downloaded1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/a575c56b-ac40-4595-9f7e-e5f1b5a09691">
<img width="573" alt="next11" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/4c37ff1c-e1d4-47f0-8b9d-e76aef49d94f">

##

Click Next and click Noted to accept the license agreement:

<img width="576" alt="next22" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/2f1a871f-040a-4b34-a2b3-201912699414">
<img width="635" alt="noted1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/607977e5-fa69-47a5-9838-022a7f2b1324">

##

Keep the default component and click Next

<img width="549" alt="compo next1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/4059d314-28a0-4ad8-bc1b-2fd15d4ebbe4">

##

Click install to begin installing Wireshark.

<img width="543" alt="install1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/84b0a7e2-d506-4abb-ab1e-dc30ecba1448">
<img width="517" alt="installing" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/bcd36ca0-9215-4720-9bcc-f304365a48df">

##

The Wireshark icon is displayed on the desktop:

<img width="507" alt="wireshark1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Lab/assets/136107996/54059887-830b-4065-8ec0-2c035bdeff54">

## Steps - Section B
To capture traffic, launch Wireshark by double-clicking the tool.

<img width="507" alt="wireshark1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/d080d47a-0dfa-4af5-bdcf-2223c5f9cd67">

##

The Wireshark interface is shown:

<img width="630" alt="wireshark interface" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/3c009ad2-a757-4ac3-a1ea-55eed0acd41b">

##

The Wireshark interface shows a network interfaces available. 

<img width="524" alt="ethernet selection1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/6cd913b9-ff94-4d14-8797-5ef811e88729">

##

To capture traffic, Select the ethernet network and click start:

<img width="506" alt="capture click1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/81693042-b0c2-431d-bb91-24442f2dbb6e">

##

Wireshark starts capturing traffic:

<img width="669" alt="captured traffic" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/9b042750-f189-430b-ac37-a48964d6b3c5">

## 
The Wireshark interface contains components that are used to interact with the packets. 
+ The Main Toolbar: It contains packet capture tools.
+ The Filter Toolbar: It is used to filter packets.
+ The Packets List Pane: Contains lists of captured packets.
+ The Packet details Pane: Contains information about each captured packet.
+ The packet Byte Pane: 
+ The Status Toolbar: It shows the profile and the packet number.

<img width="669" alt="captured trafiic11" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/0dda3d7f-eb58-4298-9a75-d818b38d6ef4">

The ***Packet List Pane*** contains seven headings namely:
+ Number(No.): The packets are arranged in numbered ascending order.
+ Time: It shows the time the packet was captured.
+ Source: The IP address of the originator of the packet.
+ Destination: The IP address of the destination of the packet.
+ Protocol: The type of protocol used by the packet.
+ length: The size of the packet.
+ Infomation(Info): It displays brief information about the packet

## Packet Analysis

***Packet No. 1***

To analyse the traffic, Packet number one is selected. Click on the packet to examine the packet in the Packet Detail Pane:

***Packet List Pane Information***

<img width="664" alt="analy11" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/01bcd1ee-2bc0-4d19-bcf7-bf5b7d620747">

From the Packet List Pane, the first packet capture was 19:33:43. The source  and destination IP addresses are 192.168.10.5 and 104.46.162.224 respectively. The IP address 198.168.10.5 is the Windows 10 VM trying to access the web server on 104.46.162.224.
From the Packet List Pane, the protocol being used for the communication Transmission Mission Protocol(TCP). The size of the packet is 1514.
The info section in the Packet List Pane shows that the captured packet is an acknowledgement(Ack) packet being sent from the source port 50268 to destination port 433, which indicates it is web traffic.

***Packet Detail Pane Information***

__Frame__: The frame contains information such as interface ID and name, Encapsulation type, date and time etc. This is usually gathered by Wireshark on the packet.

<img width="666" alt="pd fr1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/f672c88c-43b7-489f-9107-e54346716aec">

##

__Ethernet__: The Ethernet contains the source and destination Media Access Control(MAC) address. The source MAC address is 08:00:27:aa:bf:61 and the destination MAC address is 08:00:27:7e:4a:c4.

<img width="667" alt="pd et1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/dbe5726a-56c9-4e9c-bf03-21e6b2965847">

##

__Internet Protocol Version 4__: The Internet Protocol Version 4 field contains the source and destination IP address, TTL, protocol version and other important details used during the communication.

<img width="664" alt="pdipv 1png" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/d8c970f1-27be-41cb-bdeb-2ffa64069c63">

##

__Transmissin Control Protocol__: The Transmission Control Protocol field contains  the source and destination port. In this lab, the source and destination ports are 50268 and 443 respectively. An important information in the TCP is the Sequence number(1), Acknowledgement number(1) and Other Wireshark-generated fields. _Note_: The Wireshark-generated information are the ones wrapped in square brackets([]).

<img width="665" alt="pd tcp 1png" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/4079b660-5739-459f-a08f-a8ad3e29a4bd">

## Packet Filtering

To search for a specific packet or information in captured packets as they accumulate fast, filters are used to get to specific information. 

***ip.addr***

In this lab, the filter ***ip.addr == 192.168.10.5*** is used to search for all occurrences of the IP address 192.168.10.5 in the captured traffic.

<img width="666" alt="filt addr1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/006f259a-2677-4f52-8ea9-dfbcc986ab90">

***ip.src***

To filter by only the source IP address, the filter ip.src == 192.168.10.5. This filter displays all occurrences of the IP address 192.168.10.5 as a source IP address.

<img width="667" alt="ipsrc1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/63b77bec-af53-468b-8a4d-c2c45f6f4e91">

##

To search for a specific protocol such as TLS(HTTPS), FTP, TCP, SSH, UDP, HTTP and ICMP, the protocol can be entered into the  Filter Toolbar field to search for the protocol.

***tls***

In this lab, the TLS protocol is used. This filters all communication using the TLS protocol.

<img width="667" alt="fil tls1" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/c192450d-0ccf-440f-8340-a798b0c5778b">

***udp***

Packet filtering with UDP protocol.

<img width="665" alt="udp fil 1png" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/456a6abf-6d82-48fb-8890-49e5974f0e2a">







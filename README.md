# Network-Protocol-Analysis With Wireshark

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
+ The Packet byte Pane: Contains information about each captured packet.
+ The Status Toolbar: It shows the profile and displays the packet number.

<img width="669" alt="captured trafiic11" src="https://github.com/richard-acquah/Network-Protocol-Analyzers-Wireshark-Lab/assets/136107996/e26d1701-d030-477a-b8ca-cfb1b4cd7174">


The ***Packet List Pane*** contains seven headings namely:
+ Number(No.): The packets are arranged in numbered ascending order.
+ Time


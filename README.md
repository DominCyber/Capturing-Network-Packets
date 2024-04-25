# Capturing Network Packets
## Objective
The Coursera Google Cybersecurity Professional Certification Course work provides practical cybersecurity skills. This guided project utilizes a virtual machine environment to familiarize cybersecurity professionals with the WireShark network protocol analyzer GUI and packet capture analysis methodology. The project analyzes a sample .pcap file. Specfically, this project explores methodologies to potentially discover data exfiltration.

### Skills Learned
-Data exfiltration methodologies
<p>-WireShark display filter commands:</p>
<p>--by IP Address (ip.addr == ...)</p>
<p>--by source IP Address (ip.src == ...)</p>
<p>--by destintation Address (ip.dst == ...)</p>
<p>--by MAC address (eth.addr ==...)</p>
<p>--by DNS packets (udp.port == 53)</p>
<p>--by TCP packets (tcp.port == 80)</p>
<p>-by TCP traffic with text data (tcp contains "curl")</p>
<p>-WireShark display filter operators (==. contains, etc.)
<p>-Packet capture analysis:</p>
<p>--Destination IP address</p>
<p>--Arrival time</p>
<p>--Header Length</p>
<p>--Frame length</p>
<p>--MAC address</p>
<p>--Internal protocol</p>
<p>--Time to live</p>
<p>--TCP containing text data</p>

### Tools Used
-Laptop
<p>-WireShark network protocol analyzer GUI</p>
<p>-Coursera Google Cybersecurity Professional Certification</p>

### Steps
<img src="https://i.imgur.com/hikn1xJ.jpg" style="width: 200%;" alt="1">
<p><i>Ref 1: Display Filter results for IP address query</i></p>
<img src="https://i.imgur.com/7Zjb5Mx.jpg" style="width: 65%;" alt="1">
<p><i>Ref 2: Frame subtree, where attention is brought to arrival time, frame length</i></p>
<img src="https://i.imgur.com/ldNzY5m.jpg" style="width: 65%;" alt="1">
<p><i>Ref 3: Ethernet II subtree, where attention is brought to source and destination MAC addresses, and the Time to Live value</i></p>
<img src="https://i.imgur.com/Zw8gX2I.jpg" style="width: 65%;" alt="1">
<p><i>Ref 4: Transmission Control Protocol subtree, where attention is brought to source and destination port, and Flags</i></p>
<img src="https://i.imgur.com/jbl1iUO.jpg" style="width: 200%;" alt="1">
<p><i>Ref 5: Display Filter results for source IP address query</i></p>
<img src="https://i.imgur.com/zun9dkB.jpg" style="width: 200%;" alt="1">
<p><i>Ref 6: Display Filter results for destination IP address query</i></p>
<img src="https://i.imgur.com/mamNprf.jpg" style="width: 200%;" alt="1">
<p><i>Ref 7: Display Filter results for MAC Address query</i></p>
<img src="https://i.imgur.com/GWNqW6J.jpg" style="width: 200%;" alt="1">
<p><i>Ref 8: Display Filter results for DNS packet query</i></p>
<img src="https://i.imgur.com/9fMdqd0.jpg" style="width: 65%;" alt="1">
<p><i>Ref 9: Domain Name Protocol subtree, where attention is brought to the Answers dropdown denoting answering domains (opensource.google.com)</i></p>
<img src="https://i.imgur.com/kStNuqB.jpg" style="width: 200%;" alt="1">
<p><i>Ref 10: Display Filter results for TCP packet query, note time to live value 64, most likely denoting origin from a Linux machine</i></p>
<img src="https://i.imgur.com/1sGYGfB.jpg" style="width: 85%;" alt="1">
<p><i>Ref 11: Display Filter results for source TCP containing text data query</i></p>

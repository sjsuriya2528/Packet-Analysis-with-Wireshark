**# Packet-Analysis-with-Wireshark**

**🕵️‍♂️ Task 4: Packet Analysis Using Wireshark**

This task involves capturing and analyzing network traffic using Wireshark to identify suspicious or potentially malicious activities. Wireshark is a widely used network packet analyzer that allows cybersecurity analysts to inspect data packets flowing through a network in real time.

**📌 Objective**

Capture network packets

Analyze protocols like TCP, UDP, DNS, ARP, HTTP

Apply filters to identify suspicious activity

Document findings with screenshots

**🛠️ Tools Used**

Wireshark (Packet Analyzer)

Operating System: Kali Linux / Windows

Internet connection for live capture

**📥 1. Packet Capture**

I started Wireshark and selected my active network interface.
Once the capture started, packets began appearing live, showing:

Source IP

Destination IP

Protocol (TCP, UDP, DNS, ARP, HTTP)

Additional information

A screenshot of the live capture is included in the screenshots/ folder.

**🔍 2. Filters Used for Analysis**

During packet analysis, I applied the following filters:

✔ View all TCP packets
tcp

✔ View all UDP packets
udp

✔ HTTP traffic
http

✔ DNS queries
dns

✔ ARP packets (to detect spoofing)
arp

✔ Detect possible port scanning
tcp.flags.syn == 1 && tcp.flags.ack == 0

✔ Check traffic to a specific IP
ip.addr == <target-ip>

**🚨 3. Malicious Activity Detection**

I inspected the filtered packets to identify abnormal or suspicious patterns.

**⭐ Findings:**

✔ Normal traffic such as DNS queries and TCP handshakes were visible

✔ ARP table looked stable (no duplicate IP–MAC conflicts)

✔ No direct signs of port scanning during the session

✔ No unusual foreign IP connections detected

If any suspicious packets were found, they were noted and captured in screenshots.

**Conclusion**

This task helped me understand:

How network packets flow in real time

How to use Wireshark filters to isolate specific traffic

How to identify potential threats such as ARP spoofing, port scanning, and suspicious DNS queries

How to capture and document packet analysis effectively

Wireshark is a powerful tool for both networking and cybersecurity, making packet analysis a key skill in threat detection.

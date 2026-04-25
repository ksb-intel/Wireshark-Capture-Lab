# Wireshark-Capture-Lab
## Overview

<img width="1468" height="512" alt="image" src="https://github.com/user-attachments/assets/47ef19d7-dda4-40c0-9dd5-20b87bdeb54b" />

<br>

This project captures and analyzes PCAPs (network packet capture files) using Wireshark on Windows 11. The goal was to capture live key network protocols and demonstrate packet analysis using the Wireshark display filters. 

<br>

---

## Wireshark Installation

Wireshark can be installed on Windows, macOS, and Linux. To begin installing visit the [Wireshark website](https://www.wireshark.org/download.html) and download the respective installation for your operating system. More information can be found in the official  [Wireshark Documentation](https://www.wireshark.org/docs/). 


---

## Traffic Types Captured

ICMP - captured via `ping 8.8.8.8`
<br>
DNS --- captured via `nslookup google.com`
<br>
TCP 3-Way Handshake --- captured via fresh web connection
<br>
UDP --- captured through streaming Spotify
<br>
TCP Port 80 Traffic --- captured by visiting  http://neverssl.com
<br>
HTTP --- captured by visiting http://neverssl.com despite modern HTTPS enforcement
<br>


---

## Screenshots

### ICMP (Internet Control Message Protocol)

 | Captured Echo Request and Echo Reply packets by using `ping 8.8.8.8`.

<img width="1911" height="931" alt="image" src="https://github.com/user-attachments/assets/a45f06a5-2faa-46a1-9bee-15900b1ddf89" />

<br>

### DNS (Domain Name System Lookup)

| Captured DNS query and response by utilizing `nslookup`.

<img width="1912" height="843" alt="image" src="https://github.com/user-attachments/assets/a98b2e94-6539-4cad-9d48-7190967a3768" />

<br>

### TCP 3-Way Handshake

| Captured the SYN -> ACK -> ACK TCP sequence during a web connection startup. 

<img width="1910" height="928" alt="image" src="https://github.com/user-attachments/assets/145fc88b-4f6f-4a13-9730-722e62017f15" />

<br>

### UDP (User Datagram Protocol)

| Captured UDP traffic by keeping an open Spotify broadcast connection. 

<img width="1910" height="915" alt="image" src="https://github.com/user-attachments/assets/153b7332-8040-4c73-9252-121f29a6a71c" />

<br>

### TCP Port 80 Traffic

| Captured TCP packets directed to Port 80 by visiting a site specifically designed to remain unencrypted. We see the initial TCP handshake, followed by the HTTP GET request and then TCP retransmission, showing how TCP corrects errors if packets are dropped along the way.

<img width="1915" height="930" alt="image" src="https://github.com/user-attachments/assets/ea805d81-c735-4763-bc3b-487464a92b22" />

<br>

### HTTP

| Captured only the HTTP GET request. Browser asks the server for the webpage, the server says the page has moved and redirects. Then the server delivers the request via 200 OK and delivers the favicon.ico that appears in the browser tab. 

<img width="1908" height="937" alt="image" src="https://github.com/user-attachments/assets/a97164ae-8c2b-4174-9cce-c86287522b56" />

<br>

### Random Background Traffic

| Miscellaneous network traffic


<img width="1899" height="869" alt="image" src="https://github.com/user-attachments/assets/3c89e11d-95f0-413c-bdc8-4c67d6f20904" />

<br>

---

### Skills Practiced

- Packet capturing and saving
- Applying Wireshark filters for specific protocols
- Analyzing ICMP, DNS, TCP handshakes, HTTP-Traffic, and UDP
- Documenting findings and drawing conclusions on PCAPs
- Real-world troubleshooting with HTTP environments

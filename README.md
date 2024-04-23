# WireShark Project From Coursera
## Project Objective

<li>Install and set up Wireshark on Ubuntu.</li>

<li>Start a packet capture on an ethernet port and save it to file.</li>

<li>Use a display filter to detect HTTPS packets.</li>

<li>Practice Task: Start a Wireshark capture and detect HTTP packets.</li>

<li>Visit a web page and detect its IP address using a display filter.</li>

<li>Locate all HTTPS packets from a capture not containing a certain IP address.</li>

<li>Capstone Task: Use Wireshark to capture and observe ethernet packets on HTTP and HTTPS ports.</li>


## Task 1
● Install and set up Wireshark on Ubuntu:

<img src="1.png">

● To get the latest stable version of Wireshark on Ubuntu Linux, use the add-apt-repository command: sudo add-apt-repository ppa:wireshark-dev/stable

<img src="2.png">

● Wireshark should not be run as superuser for security reasons.

● The user can be added to the Wireshark group to add packet capture capabilities: sudo usermod -aG wireshark $USER

<img src="3.png">

## Task 2

### Start a packet capture on an ethernet port and save it to file:

●The wired interface includes the ethernet packet capture, which begins with ‘en’ in Wireshark.

<img src="5.png">

<img src="6.png">

●The Wireshark app includes controls to start packet capture, stop capture, save the packets to a file, and load the capture file.

<img src="7.png">

<img src="8.png">

<img src="9.png">

<img src="10.png">

●A capture can only be saved once the capture has stopped.

<img src="11.png">

<img src="12.png">

<img src="13.png">

<img src="14.png">

<img src="15.png">

<img src="16.png">




## Task 3

### Use a display filter to detect HTTPS packets:

●To display certain packets in an existing packet capture, use a display filter.

<img src="19.png">

<img src="21.png">

<img src="22.png">

<img src="23.png">

●To display only HTTPS traffic, use a filter on TCP port 443: tcp.port == 443

<img src="25.png">

<img src="28.png">

<img src="29.png">

<img src="30.png">

<img src="32.png">


## Task 4
### Visit a web page and detect its IP address using a display filter:

●A TLS handshake display filter may be used to detect a website visit in a packet list: tls.handshake.type ==1

<img src="45.png">

<img src="46.png">

<img src="47.png">

<img src="49.png">

<img src="50.png">

●The IP address is used in a filter to obtain packet information for a particular website: ip.addr == 142.251.163.105

<img src="51.png">

<img src="52.png">

<img src="53.png">

<img src="53.png">

## Task 5

### Locate all HTTPS packets from a capture not containing a certain IP address:

●A Conditional statement may be used to include and eliminate packets from a Wireshark capture: !(ip.addr == 8.43.85.97) and tcp.port == 443

<img src="59.png">

<img src="60.png">

<img src="61.png">

<img src="62.png">



●A compound conditional should include parentheses to avoid order of execution errors: !(ip.addr == 8.43.85.97) and (tcp.port == 80 or tcp.port == 443)

<img src="64.png">

<img src="71.png">

<a href="https://github.com/SalaiSwetha/Microsoft-Windows-Defender-and-Firewall-.git"> **Back to Main Page** </a>



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




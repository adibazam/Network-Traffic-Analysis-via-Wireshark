<h1>Network-Traffic-Analysis-via-Wireshark</h1>

<h2>Description</h2>
In this scenario, I'm a security analyst investigating traffic to a website.

I will analyze a network packet capture file that contains traffic data related to a user connecting to an internet site. The ability to filter network traffic using packet sniffers to gather relevant information is an essential skill as a security analyst.

I must filter the data in order to:
* identify the source and destination IP addresses involved in this web browsing session,
* examine the protocols that are used when the user makes the connection to the website and
* analyze some of the data packets to identify the type of information sent and received by the systems that connect to each other when the network data is captured.
<br />


<h2>Languages and Utilities Used</h2>

- <b>wireshark</b> 

<h2>Lab walk-through:</h2>

<p align="center">
Task 1: Filter the data for traffic associated with a specific IP address of "142.250.1.139" and inspect the packet as well. What is the protocol of the first packet in the list where the info column starts with the words 'Echo (ping) request'?<br/>
<img src="https://i.gyazo.com/e3fe33d87d17b64ce5286b496bbeaa69.png" height="80%" width="80%" alt="tcpdump"/>
<img src="https://i.gyazo.com/23034aed27ddef04e0c2602bef6bf1b3.png" height="80%" width="80%" alt="tcpdump"/>
<img src="https://i.gyazo.com/fe6e5de4595995599b69f308bbd0579c.png" height="80%" width="80%" alt="tcpdump"/>  
<br />
<br />
<p align="center">  
Task 2. Apply a basic Wireshark filter and inspect a packet for specific information <br/>
<img src="https://i.gyazo.com/cd3faa84fbcc7da2773f2e3c1ed5c6a0.png" height="80%" width="80%" alt="tcpdump"/>
<img src="https://i.gyazo.com/45586ac4bf9fdb7db16b7bfd0145acd0.png" height="80%" width="80%" alt="tcpdump"/>
<br />
<br />
<p align="center">  
Task 3. You’ll use filters to analyze specific network packets based on where the packets came from or where they were sent to. You’ll explore how to select packets using either their physical Ethernet Media Access Control (MAC) address or their Internet Protocol (IP) address. 
  Enter the following filter to select traffic to or from a specific Ethernet MAC address. This filters traffic related to one MAC address, regardless of the other protocols involved: eth.addr == 42:01:ac:15:e0:02.
  After analyzing the first packet listed, what is the protocol contained in the Internet Protocol Version 4 subtree related to MAC address 42:01:ac:15:e0:02?<br/>
<img src="https://i.gyazo.com/a153ef69fbc489b79db2e183f4fbb0a5.png"/>
<img src="https://i.gyazo.com/98150c74ba67d390c0aaab0ac3266b85.png" height="80%" width="80%" alt="tcpdump"/>
<br />
<br />

<h1>Network Traffic & Security Log Analysis<h1/>

 
<h2>Objective<h2/>
 
The objective of this lab was to analyze network traffic and system logs to identify the user responsible for suspicious SMTP activity. Wireshark was used to examine a provided capture (PCAP) file, while DHCP and security logs were analyzed to correlate the network activity with a specific device and user account.

<h2>Tools and Files<h2/>
 <ul></ul>
<li>Wireshark</li>
<li>PCAP network capture file</li>
<li>DHCP log</li>
<li>Windows Security log</li>
<li>SMTP network traffic</li>
<h2>Procedure:<h2/>

<li>Downloaded the provided files and installed Wireshark.</li>
<li>Opened the .pcap file in Wireshark to analyze the files for any malware.</li>
 <img src="https://github.com/deiondrar/Network-Traffic-Security-Log-/blob/main/Picture1.png" alt="">
<li>Applied the smtp display filter to sort through all the packets from the larger packet capture.</li>
<img src="https://github.com/deiondrar/Network-Traffic-Security-Log-/blob/main/Picture2.png" alt="">
<li>To filter the packets even more to see the rogue user the filter smtp contains “FROM” was used.</li>
 <img src="https://github.com/deiondrar/Network-Traffic-Security-Log-/blob/main/Picture6.png" alt="">

<li>Recorded the IP address associated with the suspicious network activity.</li>
 <img src="https://github.com/deiondrar/Network-Traffic-Security-Log-/blob/main/Picture3.png" alt="">

<li>Reviewed the provided DHCP log and correlated the identified IP address with the corresponding device.</li>
 <img src="https://github.com/deiondrar/Network-Traffic-Security-Log-/blob/main/Picture4.png" alt="">

<li>Compared the network, DHCP, and security log information to determine the user associated with suspicious activity.</li>
<li>Used the collected evidence to determine whether the identified activity was associated with the suspected employee.</li>
<h2>Findings:</h2>
The investigation demonstrated how network traffic can be correlated with system and DHCP logs to identify the user associated with suspicious activity. By filtering SMTP traffic in Wireshark, identifying the corresponding IP address, and comparing that information against DHCP and security logs, the responsible user account could be determined.

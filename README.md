Network Traffic & Security Log Analysis
Objective
The objective of this lab was to analyze network traffic and system logs to identify the user responsible for suspicious SMTP activity. Wireshark was used to examine a provided capture (PCAP) file, while DHCP and security logs were analyzed to correlate the network activity with a specific device and user account
Tools and Files
•	Wireshark
•	PCAP network capture file
•	DHCP log
•	Windows Security log
•	SMTP network traffic
Procedure:
•	Downloaded the provided files and installed Wireshark.
•	Opened the .pcap file in Wireshark to analyze the files for any malware.
 
•	Applied the smtp display filter to sort through all the packets from the larger packet capture. 
•	To filter the packets even more to see the rogue user the filter smtp contains “FROM” was used. 
 
•	Recorded the IP address associated with the suspicious network activity.
 
•	Reviewed the provided DHCP log and correlated the identified IP address with the corresponding device.
 
•	Compared the network, DHCP, and security log information to determine the user associated with suspicious activity.
•	Used the collected evidence to determine whether the identified activity was associated with the suspected employee.
Findings:
The investigation demonstrated how network traffic can be correlated with system and DHCP logs to identify the user associated with suspicious activity. By filtering SMTP traffic in Wireshark, identifying the corresponding IP address, and comparing that information against DHCP and security logs, the responsible user account could be determined.

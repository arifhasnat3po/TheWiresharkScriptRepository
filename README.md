# TheWiresharkScriptRepository
#Introduction
The purpose of this lab report is to analyze malicious network traffic and identify the behavior and characteristics of the malware. The specific malware analyzed in this report is a Trickbot infection, which is a banking Trojan that is often used to steal banking credentials and other sensitive information. By analyzing the traffic, we can develop countermeasures and prevent similar attacks from occurring in the future.


#Methodology
Malware Traffic Analysis package link: https://malware-traffic-analysis.net/2020/05/28/index.html 

The traffic was filtered to focus on specific protocols and ports, such as DNS, HTTP, and HTTPS on port 443.

Specific filters were applied to identify the IP address of the infected machine, the user agent, and the server used.

The TCP stream was followed to reveal specific traffic, such as a POP3 email server link, an OpenVPN password and configuration, and OpenSSH traffic.
	
HTTP filters were used to identify specific IP addresses associated with a post at packet 1496 and a file being exported using HTTP.
	
Hash decoding was used to identify the specific fingerprint of the Trickbot infection using a tool called JA3.

Results

#Step 1: Password-protected access to the malware traffic was obtained
Access to the malware traffic was obtained by using the password "infected". This allowed us to view the captured network traffic for analysis.

#Step 2: The traffic was filtered to focus on specific protocols and ports
The traffic was filtered to focus on specific protocols and ports, such as DNS, HTTP, and HTTPS on port 443. This allowed us to narrow down the traffic to specific areas of interest for analysis.

#Step 3: Specific filters were applied to identify the IP address of the infected machine, the user agent, and the server used
Filters were applied to identify the IP address of the infected machine, the user agent, and the server used. By analyzing this information, we were able to identify specific details about the malware, such as the specific version of the user agent and the server used by the malware.

#Step 4: The TCP stream was followed to reveal specific traffic
The TCP stream was followed to reveal specific traffic, such as a POP3 email server link, an OpenVPN password and configuration, and OpenSSH traffic. By following the TCP stream, we were able to analyze the specific traffic and identify the types of data being transmitted.

#Step 5: HTTP filters were used to identify specific IP addresses associated with a post at packet 1496 and a file being exported using HTTP
HTTP filters were used to identify specific IP addresses associated with a post at packet 1496 and a file being exported using HTTP. This allowed us to analyze the data being transmitted and identify potential indicators of compromise.

#Step 6: Hash decoding was used to identify the specific fingerprint of the Trickbot infection using a tool called JA3
Hash decoding was used to identify the specific fingerprint of the Trickbot infection using a tool called JA3. By using this tool, we were able to identify the specific fingerprint of the malware and determine that it was a Trickbot infection.

#Results
By following the methodology outlined above, the following results were obtained:
DNS-lookup -
 ![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/963db41d-9d07-4869-a30a-12d59b57995e)


#IP address of the infected machine
 ![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/ca9b3651-a63b-482e-977f-c187f4feab80)

#A POP3 email server link, an OpenVPN password and configuration, and OpenSSH traffic were identified.
Specific IP addresses associated with a post

 ![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/f3ea07a7-65b1-48a4-8341-88bb7fa21e21)
 ![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/43d34f9d-8e32-4d16-8e07-8e446d4e301d)

#Specific IP addresses associated with a post at packet 1496
![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/994fd190-715a-4828-b2f6-3bb6898e1ebe)

#FILE EXPORT OBJECT HTTP 

#Filter: frame contains “imgpaper” -->it’s an executable file
 ![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/575bb4eb-86ed-4561-af3f-77e97f347b6a)


#From the Transmission control security layer, we can find the JA3 fingerprint  
 ![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/017fbceb-f92c-43f0-a9cc-196f2ff2ca7f)

#From the following link we can verify that this is trickbot malware: https://github.com/salesforce/ja3
 ![image](https://github.com/arifhasnat3po/TheWiresharkScriptRepository/assets/63786513/2f0cabb1-715c-4396-a155-bcc7ee84f37a)

The results of this analysis show that the malware was able to bypass security measures and infect the machine. By analyzing the traffic, we can develop countermeasures to prevent similar attacks from occurring in the future. Specifically, we can update security protocols to use more secure versions of TLS, monitor for suspicious network traffic, and block known IP addresses associated with the Trickbot infection.

In conclusion, this lab report demonstrates the importance of analyzing malicious network traffic in order to identify the behavior and characteristics of malware. By doing so, we can develop countermeasures and prevent similar attacks from occurring in the future. In this case, the analysis identified a Trickbot infection, which is a banking Trojan that is often used to steal banking credentials and other sensitive information.

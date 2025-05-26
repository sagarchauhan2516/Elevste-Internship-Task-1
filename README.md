# Elevate-Internship-Task-1
This is the solution of the Task 1 for my internship
I have Scanned my ip address for the Open ports and analyzed the results.

# The results are as,
PORT     STATE SERVICE
135/tcp  open  msrpc
139/tcp  open  netbios-ssn
445/tcp  open  microsoft-ds
7070/tcp open  realserver

# Common services running on the port and potential security risks for these ports 
Port	Protocol	Service	       Description	                                                                                 Security Risk
135	  TCP	      MSRPC	         Microsoft Remote Procedure Call. Used for DCOM services and Windows services communications.	 Exploitable by malware like Blaster worm; should not be exposed to internet.
139	  TCP	      NetBIOS-SSN	   NetBIOS Session Service. Used for Windows File and Printer Sharing (legacy).	                 Can leak system info and be exploited for SMB relay attacks.
445	  TCP	      Microsoft-DS	 SMB over TCP. Used by Windows for file sharing, printer sharing, and Active Directory.	       Vulnerable to ransomware (e.g., WannaCry, EternalBlue).
7070	TCP	      RealServer	   RealNetworks streaming media server (used by RealPlayer).	                                   Often unused today; old versions may contain unpatched vulnerabilities.

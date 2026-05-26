#Raptor-Hunty — Stealth Recon & Vulnerability Assessment Framework

Raptor-Hunty is an automated penetration testing tool built on top of Metasploit Framework and Nmap. Instead of running commands manually one by one, this tool guides you through the entire reconnaissance process with an interactive shell — from entering your target IP all the way to a structured report saved automatically on your Desktop.

What it does:

-Asks you to choose language (Spanish or English) and target OS type
-Lets you choose the scan aggression level: Noisy (-T4), Semi-noisy (-T3), or Quiet stealth mode (-T2)
-Runs Nmap through Metasploit's db_nmap so all results go directly into the MSF database
-Detects open services and automatically suggests the right Metasploit auxiliary module to use for each one (SSH, HTTP, SMB, FTP, RDP)
-Flags possible CVEs based on the detected service versions
-Saves a full report to your Desktop at the end of every scan
-Validates your inputs, checks file integrity with SHA-512, and only runs for authorized users

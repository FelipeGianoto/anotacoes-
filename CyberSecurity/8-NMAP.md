<h1> NMAP </h1>

Nmap é uma ferramenta para descobrir host e serviços abertos em uma rede de computador.
Nmap is an free, open-source and powerful tool used to discover hosts and services on a computer network.

<b> nmap -sV</b> <u>machinesIp</u>

nmap flag
Description
-sV
Attempts to determine the version of the services running
-p <x> or -p-
Port scan for port <x> or scan all ports
-Pn
Disable host discovery and just scan for open ports
-A
Enables OS and version detection, executes in-build scripts for further enumeration 
-sC
Scan with the default nmap scripts
-v
Verbose mode
-sU
UDP port scan
-sS
TCP SYN port scan

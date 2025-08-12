# Nmap

### What Nmap can do?
- simply scan a server or IP to find what ports are open or devices in that lan also find out the version of the services, the OS + version.

### Command
(All command like (-sS -O ...) are writen between nmap comand the the IP)
- nmap 192.168.1.0/24 : to scan the whole netword and find the devies on this lan + "-sn"
- If we want to scan server ports we use "nmap (server IP)" 
- If need to see all ports we use "-p-"" before the server IP
- To see the version of services use "-sV" 
- To know the OS of the server we use "-O"
- To do stealth scan use the "-sS" 
- "-sC" you can use this promot in nmap to run scripts that's help you to find much more info and much more than that.
>Stealth scan : Baiscally is to send SYN when the server send SYN/ACK we do a reset (on some old version the logs might not be saved because the process didn't complete) all this prosess to have no logs of this scan.
- "-Pn" used in no ping scan
- Aggressive scan"-A" equal to "-O -sV -sC" all together
- "--scrip=..." to run specific script
- "-T(0-5)" we use this to speed up the process we can use the numberes from 0-5 
- "-f" fragmenting the packet
- "-g" do the scaning from specific port



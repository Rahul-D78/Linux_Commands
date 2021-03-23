## 10 things to check when you are initially working on a linux server :-

## __Check if anybody unboard :-__
```$ who -Hu```
```$grep sh$ /etc/passwd```
## __Check the system info (software and hardware):-__
 ```$dmidecode -s system-manufacture```
```$dmidecode -s system-product-name```
```$lshw```
```$lscpu```
```$cat /proc/meminfo```
```$cat /proc/cpuinfo```
```$uptime```
## __Check for the network info :-__
```$ifconfig -a```
```$ethtool wlan0```
```$lshw```
```$lspci```
* Additionally you need to know a lot of networking tools to complete your desire task :-
1. wireshark
2. netstat
3. netcat
4. iptables
5. nat
6. nmcli
```$netstat -anp```
```$netstat -tulpn```
```$iwconfig```
```$ip addr```
```$iptables -L -n```
```$cat /etc/resolv.conf```
* Use nmcli to configure the network manager
```nmcli d wifi list ifname wlan0```
## __Check and install the required packages :-__
```$apt list```
```$apt isntall```
## __Check for process info :-__
```$pstree -pa 1```
```$ps aux```
you can also use grep command to check for any specific package
```$ps aux | grep nginx```
```$ps auxf```
```$ps -ef```
## __kernel info :-__
kernel is the bridge between software and hardware and it's main task is process, memory, network management 
```$uname -r```
```$lsmod```
## __check for log :-__
```$journalctl```
```$dmesg```




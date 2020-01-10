# Priv Esc

## OS ENUMERATION


   

* **uname -a**	 || *Print all available system information*
* **uname -r** ||	*Kernel release*
* **uname -n** ||	*System hostname*
* **hostname**	|| *As above*
* **uname -m**	|| *Linux kernel architecture (32 or 64 bit)*
* **cat /proc/version** ||	*Kernel information*
* **cat /etc/*-release** || *Distribution information*
* **cat /etc/issue**	|| *As above*
* **cat /proc/cpuinfo**	|| *CPU information*
* **df -a**	|| *File system information*

## User Enumeration

* **for i in $(cat /etc/passwd 2>/dev/null| cut -d":" -f1 2>/dev/null);do id $i;done 2>/dev/null** || *lists UIDs and groups*

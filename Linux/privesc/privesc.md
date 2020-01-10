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
* **sudo -V** || *sudo version*
* **find / -name %program_name% 2>/dev/null** || *find a program*

## User Enumeration

* **for i in $(cat /etc/passwd 2>/dev/null| cut -d":" -f1 2>/dev/null);do id $i;done 2>/dev/null** || *lists UIDs and groups*
* **sudo -l, cat /etc/sudoers** || view sudo permissions of the current users
* **finger, pinky, users, who -a, id** || *curently logged in users*

## File Esc

* **find . -type f -exec grep -i -I "PASSWORD" {} /dev/null \;** || *find passwords in file*
* **grep --color=auto -rnw '/' -ie "PASSWORD" --color=always 2> /dev/null** || *same as above*

## Priv Escaping

* **Nmap
* **Vim
* **find
* **Bash
* **More
* **Less
* **Nano
* **cp

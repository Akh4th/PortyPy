# PortyPy - Python Port Scanner (Python3 and above)
 Run this script in order to scan ports of hosts inside your network !<br/>
 In case of troubles type --help or -h to get the help menu.

# Usage
--port, -p : select a single port to check, Example : python3 PortyPy.py 10.10.11.13 --port 80 <br/>
--ports, -P : select a port range to check, Example : python3 PortyPy.py 10.10.11.13 --ports 100 <br/>
--verbose, -v : Prints the process verbosity, Example : python3 PortyPy.py 10.10.11.13 -P 100 -v <br/>
--Output, -O : Prints the output into a file, Example : python3 PortyPy.py 10.10.11.13 --ports 100 -O 100_ports.txt <br/>
--get_version, -Gv : Prints estimated services version, Example : python3 PortyPy.py 10.10.11.13 --port 22 -Gv <br/>
--check_host, -Ch : Ping host to check if alive, Example : python3 PortyPy.py 10.10.11.13 --ports 100 -Ch -Gv -v <br/>
--get_os, -GO : Trying to get host's operation system, Example : python3 PortyPy.py 10.10.11.13 -Ch -GO <br/>
--fast_scan, -Fs : Scan fewer port then the usual, Example : python3 PortyPy.py 10.10.11.13 -Fs -Gv -GO -v
 
 # Examples
 python3 PortyPy.py 10.10.11.103 --ports 1200 -Gv --Output scan.txt --verbose --check_host<br/>
 python3 PortyPy.py 10.10.11.1-100 -P 100 -O scan.txt<br/>
 python3 PortyPy.py 10.10.11.13 , 10.10.11.15 , 10.10.11.19 --port 22 --Output scan.txt --get_version

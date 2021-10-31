# pyposc
Multithreaded port scanner written in Python.

## Requirements
* pyfiglet==0.8.post1
* termcolor==1.1.0

Use the command 'pip install -r requirements.txt' to install all requirements at once.

## Usage
1. Run 'python pyposc.py'
1. Enter an IP address in the format (192.168.1.1)
2. Enter a single port (a), multiple ports (a, b, c) or a range of ports (a-b)
3. Enter number of threads to use for the scanning

## Changelog
###### Version 1.1:
* Fixed a bug where open ports that couldn't be translated to a service, would be considered closed. It now shows the port as open but the service running on it as 'unknown'.
###### Version 1.2
* Added a timer that will print out how many seconds the scan took to finalize at the end of a scan.
* Fixed a bug where the last port in a port range wouldn't get scanned.


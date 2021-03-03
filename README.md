# MYDIG
A dns resolver
INTRODUCTION:
This program is a resolver takes input domain name, and output the IP address, query time and date of query.
The resolver resolves this query by first contacting the root server, the top-level domain, all the way until the authoritative name server. If ‘cname’ record returned, output ‘cname’ record and keep resolve the “cname” until get a ‘A’ record.

External library used: dnspython

Instruction of how to run the code:
1.	If you have pycharm, use pycharm to open and run the mydig.py
2.	The command prompt: use ‘cd’ command open the file containing the mydig.py, then enter “python mydig.py” to run the code.

After running code, it output “Enter a domain name: “, then input a domain name the user wished to resolve, and the program will output the question section, the answer section, query time and date like below: 
Enter a domain name: www.cnn.com
QUESTION SECTION:
www.cnn.com   IN  A
ANSWER SECTION: 
www.cnn.com. 300 IN CNAME turner-tls.map.fastly.net.
turner-tls.map.fastly.net. 30 IN A 151.101.209.67
Query time: 8.6 msec
WHEN: Sat Feb 27 17:28:26 2021



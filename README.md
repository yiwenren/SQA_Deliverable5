# IS 2545 SQA_Deliverable5 Secutiry Testing<br>

## Vulnerability SQL Injection<br>
1. What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
<br>
This vulnerability attacks integrity, because the SQL injection may be possible.<br>
2. What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?<br>
	Fabrication and modification can exploit this vulnerability. The attackers could gain access to the admin system to delete, insert and make up data. <br>
3. Are attacks that exploit this vulnerability active or passive?<br>
	Attacks are active.<br>
4. What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?<br>
	It will cause data loss and unauthorized access. Because the attackers could get access to the admin system due to the vulnerability, they are able to delete, modify and add new data into the system. They can also easily get some confidential information from the admin page.<br>
5. What steps should the development team take to fix this vulnerability?<br>
•	Set visit limitations for users. For example, add a “role” column for user and administrators to give administrators higher privilege.<br>
•	Set some rules for the username and password. For instance, the username must include uppercase, lowercase, and can only start with character. <br> 
### In addition to the answers to these questions, the following information should also be provided.
1)	The URL of the website with the described vulnerability.   http://demo.testfire.net/bank/login.aspx
2)	Steps taken to exploit the vulnerability.
•	Open the website: http://demo.testfire.net/bank/login.aspx
•	Input “ZAP' OR '1'='1'--” in the username box
•	Input whatever you want for password
•	Press the Login button
•	Then enter the admin page.<br>
3)	A screenshot (if applicable) of the vulnerability.









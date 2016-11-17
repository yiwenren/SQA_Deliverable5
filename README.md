# IS 2545 SQA_Deliverable5 Secutiry Testing<br>

## Vulnerability SQL Injection<br>
#### 1. What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
<br>
This vulnerability attacks integrity, because the SQL injection may be possible.<br>
#### 2. What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?<br>
	Fabrication and modification can exploit this vulnerability. The attackers could gain access to the admin system to delete, insert and make up data.
#### 3. Are attacks that exploit this vulnerability active or passive?<br>
	Attacks are active.
#### 4. What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?<br>
	It will cause data loss and unauthorized access. Because the attackers could get access to the admin system due to the vulnerability, they are able to delete, modify and add new data into the system. They can also easily get some confidential information from the admin page.
#### 5. What steps should the development team take to fix this vulnerability?<br>
•	Set visit limitations for users. For example, add a “role” column for user and administrators to give administrators higher privilege.<br>
•	Set some rules for the username and password. For instance, the username must include uppercase, lowercase, and can only start with character. <br>
### In addition to the answers to these questions, the following information should also be provided.
#### 1.	The URL of the website with the described vulnerability.
	http://demo.testfire.net/bank/login.aspx
#### 2.	Steps taken to exploit the vulnerability.
•	Open the website: http://demo.testfire.net/bank/login.aspx<br>
•	Input “ZAP' OR '1'='1'--” in the username box<br>
•	Input whatever you want for password<br>
•	Press the Login button<br>
•	Then enter the admin page.<br>
#### 3.	A screenshot (if applicable) of the vulnerability.
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/1_1.png)
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/1_2.png)<br><br><br>


## Remote OS command injection<br>
#### 1. What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
<br>
The vulnerability attacks the confidentiality part of the InfoSec Triad, for it shows some information to unauthorized users.<br>
#### 2. What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?<br>
	Interception. Interception can attack on confidentiality.
#### 3. Are attacks that exploit this vulnerability active or passive?<br>
	Attacks are active.
#### 4. What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?<br>
	Unauthorized access would be lost due to exploiting this vulnerability. The reputation will be damaged because some important data may be leaked out. 
#### 5. What steps should the development team take to fix this vulnerability?<br>
•	For any data that will be used to generate a command to be executed, keep as much of that data out of external control as possible. For example, in web applications, this may require storing the command locally in the session's state instead of sending it out to the client in a hidden form field.
<br>
•	Run codes in a "jail" or similar sandbox environment that enforces strict boundaries between the process and the operating system.  This may effectively restrict which files can be accessed in a particular directory or which commands can be executed by your software.
 <br>
•	Use a vetted library or framework that does not allow this weakness to occur or provides constructs that make this weakness easier to avoid.<br>
### In addition to the answers to these questions, the following information should also be provided.
#### 1.	The URL of the website with the described vulnerability.
	http://www.webscantest.com/osrun/whois.php
#### 2.	Steps taken to exploit the vulnerability.
•	Open the website: http://www.webscantest.com/osrun/whois.php<br>
•	Input “ZAP&cat /etc/passwd&” in the lookup box<br>
•	Press the Lookup button<br>
•	Some private data will be shown on screen<br>
#### 3.	A screenshot (if applicable) of the vulnerability.
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/2.png)<br><br><br>




## Vulnerability SQL Injection<br>
#### 1. What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
<br>
This vulnerability attacks integrity, because the SQL injection may be possible.<br>
#### 2. What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?<br>
	Fabrication and modification can exploit this vulnerability. The attackers could gain access to the admin system to delete, insert and make up data.
#### 3. Are attacks that exploit this vulnerability active or passive?<br>
	Attacks are active.
#### 4. What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?<br>
	It will cause data loss and unauthorized access. Because the attackers could get access to the admin system due to the vulnerability, they are able to delete, modify and add new data into the system. They can also easily get some confidential information from the admin page.
#### 5. What steps should the development team take to fix this vulnerability?<br>
•	Set visit limitations for users. For example, add a “role” column for user and administrators to give administrators higher privilege.<br>
•	Set some rules for the username and password. For instance, the username must include uppercase, lowercase, and can only start with character. <br>
### In addition to the answers to these questions, the following information should also be provided.
#### 1.	The URL of the website with the described vulnerability.
	http://demo.testfire.net/bank/login.aspx
#### 2.	Steps taken to exploit the vulnerability.
•	Open the website: http://demo.testfire.net/bank/login.aspx<br>
•	Input “ZAP' OR '1'='1'--” in the username box<br>
•	Input whatever you want for password<br>
•	Press the Login button<br>
•	Then enter the admin page.<br>
#### 3.	A screenshot (if applicable) of the vulnerability.
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/1_1.png)
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/1_2.png)









# IS 2545 SQA_Deliverable5 Secutiry Testing<br>

## Vulnerability SQL Injection<br>
#### 1. What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
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
•	Then you will enter the admin page.<br>
#### 3.	A screenshot (if applicable) of the vulnerability.
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/1_1.png)
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/1_2.png)<br><br><br>


## Vulnerability Remote OS command injection<br>
#### 1. What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
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




## Vulnerability Cross Site Scripting (Reflected)<br>
#### 1. What part of the InfoSec Triad does this vulnerability attack (confidentiality, integrity, or availability)?
The confidentiality, integrity and availability will be attacked by this vulnerability attack.<br>	
Cross-site Scripting (XSS) is an attack technique that involves echoing attacker-supplied code into a user's browser instance. When an attacker gets a user's browser to execute his/her code, the code will run within the security context (or zone) of the hosting web site. With this level of privilege, the code has the ability to read, modify and transmit any sensitive data accessible by the browser. 
<br>
#### 2. What kind of security attack can exploit this vulnerability (interruption, interception, modification, or fabrication)?<br>
Interruption, interception and modification can exploit this vulnerability.
#### 3. Are attacks that exploit this vulnerability active or passive?<br>
Attacks are active.
#### 4. What business value would be lost due to exploiting this vulnerability (data loss, unauthorized access, denial of service, etc)?<br>
It will cause data loss, unauthorized access and the denial of service. Firstly, the private data may be read, modified and transmitted by attackers. Secondly, the information of user account may be stolen by cookie theft. Thirdly, due to this vulnerability, users’ browsers may be redirected to another location, or possibly shown fraudulent content delivered by the web site they are visiting. That cause denial of service for users.
#### 5. What steps should the development team take to fix this vulnerability?<br>
•	Use a vetted library or framework that does not allow this weakness to occur or provides constructs that make this weakness easier to avoid.<br>
•	For every web page that is generated, use and specify a character encoding such as ISO-8859-1 or UTF-8. When an encoding is not specified, the web browser may choose a different encoding by guessing which encoding is actually being used by the web page. This can cause the web browser to treat certain sequences as special, opening up the client to subtle XSS attacks. <br>
•	To help mitigate XSS attacks against the user's session cookie, set the session cookie to be HttpOnly. In browsers that support the HttpOnly feature (such as more recent versions of Internet Explorer and Firefox), this attribute can prevent the user's session cookie from being accessible to malicious client-side scripts that use document.cookie.<br>
### In addition to the answers to these questions, the following information should also be provided.
#### 1.	The URL of the website with the described vulnerability.
	http://testaspnet.vulnweb.com/ReadNews.aspx?NewsAd=javascript%3Aalert%281%29%3B&id=0
#### 2.	Steps taken to exploit the vulnerability.
•	Open the website: http://testaspnet.vulnweb.com/ReadNews.aspx?NewsAd=javascript%3Aalert%281%29%3B&id=0<br>
•	A alert window(as the following screenshot) will pop up.<br>

#### 3.	A screenshot (if applicable) of the vulnerability.
![](https://github.com/yiwenren/SQA_Deliverable5/blob/master/3.png)









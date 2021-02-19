# Exploit Title: Beauty Parlour Management System 1.0 - 'Add Services' Cross-Site Scripting
# Date: 19/2/2021
# Exploit Author: Thinkland Security Team
# Vendor Homepage: https://phpgurukul.com/beauty-parlour-management-system-using-php-and-mysql/
# Software Link: https://phpgurukul.com/wp-content/uploads/2019/08/Beauty-Parlour-Management-System.zip
# Version :  V 1.0
# Vulnerability Type: Cross-site Scripting
# Tested on Windows 10 、XAMPP
# This application is vulnerable to cross-site scripting vulnerability.
# Vulnerable script:


1.go to http://localhost/bpms/admin/ Sign in.  
2.go to http://localhost/bpms/admin/add-services.php，Click on  Services —— Add Services，Fill in Services name <img src=1 onerror=alert(/xss/)>，Click on Add.  
3.Click on  Manage Services，You will see your Javascript code executed.  
![image](https://github.com/BigTiger2020/Beauty-Parlour-Management-System/blob/main/xss3.png)  
# Vulnerability proof  
![image](https://github.com/BigTiger2020/Beauty-Parlour-Management-System/blob/main/xss1.png)  
![image](https://github.com/BigTiger2020/Beauty-Parlour-Management-System/blob/main/xss2.png)    



# Exploit Title: Beauty Parlour Management System 1.0 - 'Service Name' SQL Injection
# Google Dork: N/A
# Date: 19/2/2021
# Exploit Author: Thinkland Security Team
# Vendor Homepage: https://phpgurukul.com/beauty-parlour-management-system-using-php-and-mysql/
# Software Link: https://phpgurukul.com/wp-content/uploads/2019/08/Beauty-Parlour-Management-System.zip
# Version: V 1.0 
# Tested on: Windows、XAMPP

# Identify the vulnerability
1. go to http://localhost/bpms/admin/ and login with your account
2. then go to http://localhost/bpms/admin/edit-services.php?editid=17 
3. Save the packet data as 3.txt  
![image](https://github.com/BigTiger2020/Beauty-Parlour-Management-System/blob/main/sql1.png)   
![image](https://github.com/BigTiger2020/Beauty-Parlour-Management-System/blob/main/sql2.png)   
# Vulnerability proof    
![image](https://github.com/BigTiger2020/Beauty-Parlour-Management-System/blob/main/sql3.png)   
